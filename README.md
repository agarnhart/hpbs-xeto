# HPBS Xeto Library

Xeto schema library implementing the **High Performance Building Standard (HPBS)** for Project Haystack.

## About HPBS

The [High Performance Building Standard (HPBS)](https://dfcm.utah.gov/construction-management/high-performance-building-program/) is a comprehensive construction standard developed by the Utah Division of Facilities Construction and Management (DFCM). HPBS defines requirements for building automation systems, including point naming conventions, data collection intervals, and equipment modeling.

This Xeto library implements the HPBS conventions as defined in the [HPBS Appendix F - Analytic Points and Tagging Standard](https://dfcm.utah.gov/wp-content/uploads/HPBS-Appendix-F-Analytic-Points-and-Tagging-6-17-19.xlsx), providing standardized point types, equipment templates, and system definitions for Haystack-compatible building automation.

## Design Philosophy

This library follows a **thin extension** approach:

1. **Extend, don't replace** - All types inherit from standard Haystack types
2. **Preserve interoperability** - HPBS points remain queryable with standard Haystack queries
3. **Add value, not complexity** - Only include HPBS-specific conventions that provide real benefit
4. **Composition over inheritance** - Add HPBS defaults without deep hierarchies

## What This Library Provides

### History Collection Presets

Standardized history collection intervals for different point types:

| Mixin | Mode | Interval | Use Case |
|-------|------|----------|----------|
| `HpbsHisCov` | COV | 24hr | Commands, setpoints, status points |
| `HpbsHisSampled` | Sampled | 10min | Zone sensors, secondary equipment |
| `HpbsHisSampledMajor` | Sampled | 5min | Major equipment sensors |
| `HpbsHisConsumption` | Consumption | 10min | Submeters |
| `HpbsHisConsumptionMajor` | Consumption | 5min | Main meters |

### Unit Preferences

HPBS uses imperial units:

| Domain | Unit | Mixin |
|--------|------|-------|
| Temperature | `°F` | `HpbsTempUnits` |
| Air pressure | `inH₂O` | `HpbsAirPressureUnits` |
| Water pressure | `psi` | `HpbsWaterPressureUnits` |
| Air flow | `cfm` | `HpbsAirFlowUnits` |
| Water flow | `gal/min` | `HpbsWaterFlowUnits` |
| Humidity | `%RH` | `HpbsHumidityUnits` |
| CO2 | `ppm` | `HpbsCo2Units` |
| Gas volume | `ft³` | `HpbsGasVolumeUnits` |
| Gas energy | `therm` | `HpbsGasEnergyUnits` |

### NavName Conventions

Consistent abbreviated display names for points:

| Point Type | NavName Example |
|------------|-----------------|
| Zone Temperature | `ZnTemp` |
| Discharge Air Temp | `DaTemp` |
| Chilled Water Valve | `ChwVlvCmd` |
| Supply Fan Speed | `SfSpd` |
| Boiler Run Status | `BlrRunSts` |

## Library Structure

### Layered Architecture

The library uses a two-layer architecture:

| Layer | File Pattern | Purpose |
|-------|--------------|---------|
| Placeholder | `ph.*.xeto` | Generic base specs intended for upstream contribution to Project Haystack |
| HPBS Implementation | `*.xeto` | HPBS-specific specs with colors, navNames, and history settings |

### Core Files

| File | Description |
|------|-------------|
| `lib.xeto` | Library metadata and dependencies |
| `points.xeto` | Base point types, color mixins, and history presets |

### Point Type Files

| File | Contents |
|------|----------|
| `air.xeto` | Air temperature, humidity, flow, pressure, CO2 points |
| `water.xeto` | Water temperature, flow, pressure, volume, energy (HW, CHW, CW) |
| `fans.xeto` | Fan run/status, speed, VFD points (supply, return, exhaust, relief) |
| `valves.xeto` | Valve position/command points (heating, cooling, bypass, isolation) |
| `dampers.xeto` | Damper position points (OA, RA, EA, mixed, economizer, zone) |
| `pumps.xeto` | Pump run/speed points (HW, CHW, CW, DHW, booster) |
| `stages.xeto` | Staging points (heating, cooling stages) |
| `boiler.xeto` | Boiler-specific staging and control points |
| `chiller.xeto` | Chiller-specific staging, load, and oil system points |
| `compressor.xeto` | Compressor staging and run points |
| `cooling-tower.xeto` | Cooling tower staging and control points |
| `occupancy.xeto` | Occupancy, schedule, override, lockout, alarm points |
| `electrical.xeto` | Electrical metering points (energy, power, demand) |
| `naturalgas.xeto` | Natural gas metering points (flow, volume, energy) |
| `steam.xeto` | Steam system points (flow, pressure, temperature, energy) |
| `dhw.xeto` | Domestic hot water points |
| `alarms.xeto` | Equipment and system alarm points |
| `heatexchanger.xeto` | Heat exchanger temperature points |

### Placeholder Files (for upstream contribution to ph xeto libraries)

| File | Contents |
|------|----------|
| `ph.point_air.xeto` | Generic air point placeholders |
| `ph.point_water.xeto` | Generic water point placeholders |
| `ph.point_fan.xeto` | Generic fan point placeholders |
| `ph.point_valve.xeto` | Generic valve point placeholders |
| `ph.point_damper.xeto` | Generic damper point placeholders |
| `ph.point_pump.xeto` | Generic pump point placeholders |
| `ph.point_boiler.xeto` | Generic boiler point placeholders |
| `ph.point_chiller.xeto` | Generic chiller point placeholders |
| `ph.point_compressor.xeto` | Generic compressor point placeholders |
| `ph.point_cooling-tower.xeto` | Generic cooling tower point place.olders |
| `ph.point_stages.xeto` | Generic staging point placeholders |
| `ph.point_misc.xeto` | Miscellaneous point placeholders |
| `ph.point_co2.xeto` | CO2 point placeholders |
| `ph.point_weather.xeto` | Weather point placeholders |
| `ph.point_systems.xeto` | Placeholder equipment specs |
| `ph.equip.xeto` | Placeholder equipment specs |

### Equipment and System Files

| File | Description |
|------|-------------|
| `equips.xeto` | Equipment types with point profiles (AHU, VAV, boiler, chiller, etc.) |
| `systems.xeto` | Distribution system types (chilled water, hot water, steam, condenser water) |


## Point Type Coverage

### Air Points (~80 types)
- Zone, discharge, mixed, return, outside, inlet air temperatures
- Zone, discharge, return, outside humidity
- Zone, discharge, return, outside, exhaust, mixed air flow
- Zone, discharge, building air pressure
- Zone, discharge, return CO2
- Weather (wet bulb, dew point, freeze stat)

### Water Points (~50 types)
- Hot water (entering, leaving, supply, return, delta-T)
- Chilled water (entering, leaving, supply, return, delta-T)
- Condenser water (entering, leaving, supply, return)
- Domestic hot water (supply, return)
- Flow, pressure, differential pressure, volume, energy

### Fan Points (~40 types)
- Supply, return, exhaust, relief, cooling tower fans
- Run command/status, speed sensor/command
- VFD frequency, fault, enable
- Power and energy

### Valve Points (~35 types)
- Hot water, chilled water, condenser water valves
- Heating, cooling, preheat, reheat valves
- Bypass and isolation valves
- Steam and gas valves
- Domestic hot water valves

### Damper Points (~30 types)
- Outside air, return air, exhaust, relief dampers
- Mixed air, economizer dampers
- Zone/VAV dampers with min/max setpoints
- Discharge, bypass dampers
- Fire/smoke dampers

### Pump Points (~40 types)
- Hot water, chilled water, condenser water pumps
- Primary and secondary pumps
- Domestic hot water recirculation pumps
- Booster pumps
- Power, energy, VFD points

### Staging Points (~40 types)
- Heating/cooling stages (electric, gas, DX)
- Compressor stages
- Boiler/chiller staging and control
- Cooling tower staging
- Lead/lag sequencing

### Occupancy Points (~30 types)
- Zone occupancy sensor/command
- Operating mode points
- Schedule points (optimal start)
- Override and lockout points
- DCV points
- Alarm points

### Metering Points (~25 types)
- Natural gas (flow, volume, energy, pressure)
- Electrical (energy, power, demand)
- Steam (flow, pressure, temperature, energy)
- Building and equipment submeters

### Equipment Types (~40 types)
- Air handlers (AHU, RTU, MAU, DOAS)
- VAV terminals (standard, reheat, fan-powered)
- Boilers (hot water, steam, condensing)
- Chillers (air-cooled, water-cooled, centrifugal, screw)
- Cooling towers (open, closed)
- Fan coil units (2-pipe, 4-pipe)
- Computer room (CRAC, CRAH)
- Heat pumps, heat exchangers
- Meters (electric, gas, water, BTU, steam)

### System Types
- Chilled water systems
- Hot water systems
- Steam systems
- Condenser water systems
- Domestic hot water systems

## Equipment Point Profiles

Each equipment type defines a `points: {}` block specifying which point types typically apply to that equipment. This provides:

- **Self-documenting templates** - Equipment types show exactly which points are expected
- **No duplication** - References existing point types instead of creating equipment-specific variants
- **Flexibility** - All points are optional (`?`) - instances only include what they have

### Slot Naming Convention

Slot names in `points: {}` blocks match the point type's `navName` abbreviation:

| Slot Name | Point Type | NavName |
|-----------|-----------|---------|
| `daTemp` | `HpbsDischargeAirTempSensor` | `DaTemp` |
| `sfCmd` | `HpbsSupplyFanRunCmd` | `SfCmd` |
| `chwVlvCmd` | `HpbsChilledWaterValveCmd` | `ChwVlvCmd` |
| `znTemp` | `HpbsZoneAirTempSensor` | `ZnTemp` |

### Equipment Point Counts

| Equipment | Points | Key Categories |
|-----------|--------|----------------|
| `HpbsAhu` | ~30 | Air temps, fans, dampers, valves, safety |
| `HpbsVav` | ~10 | Zone temp/flow, damper, occupancy |
| `HpbsVavReheat` | ~13 | VAV + reheat valve, discharge temp |
| `HpbsBoiler` | ~14 | HW temps, staging, gas, enable |
| `HpbsChiller` | ~15 | CHW/CW temps, staging, power |
| `HpbsCoolingTower` | ~17 | Fans, temps, staging, isolation |
| `HpbsFcu` | ~11 | Zone temp, fan, valves |

## How to use these libraries

- **As a user**
  - Install & enable the library (`hpbs`) in your [Haxall](https://github.com/haxall/haxall) project.
  - Declare equipment and points using the provided Hpbs types, extending abstract base types (such as `HPBSAhu`) for project-specific variants.

- **As a contributor**
  - Prefer extending or composing existing Hpbs traits/types instead of duplicating semantics.
  - Follow existing naming and history conventions within the hpbs libraries.

### Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details on:

- Development setup and guidelines
- Code style and naming conventions
- Pull request process
- Types of contributions we accept

### Example: AHU Point Profile

```xeto
HpbsAhu: Ahu {
  points: {
    // Air temperatures
    daTemp: HpbsDischargeAirTempSensor?
    daTempSp: HpbsDischargeAirTempSp?
    maTemp: HpbsMixedAirTempSensor?
    raTemp: HpbsReturnAirTempSensor?
    oaTemp: HpbsOutsideAirTempSensor?

    // Supply fan
    sfCmd: HpbsSupplyFanRunCmd?
    sfSts: HpbsSupplyFanRunSensor?
    sfSpd: HpbsSupplyFanSpeedSensor?

    // Dampers
    oaDmprCmd: HpbsOutsideAirDamperCmd?
    raDmprCmd: HpbsReturnAirDamperCmd?

    // Valves
    chwVlvCmd: HpbsChilledWaterValveCmd?
    hwVlvCmd: HpbsHeatingValveCmd?
  }
}
```

### Using Pre-composed Types

```xeto
// Use HPBS types directly - all Haystack queries still work
myZoneTemp: HpbsZoneAirTempSensor {
  equipRef: @my-vav
}

myChwValve: HpbsChilledWaterValveCmd {
  equipRef: @my-ahu
}
```

### Using Equipment Templates

Equipment types define expected points - just instantiate what you have:

```xeto
// Create an AHU with its points
myAhu: HpbsAhu {
  dis: "AHU-1"
  siteRef: @my-site
}

// Points reference the equipment - the equipment's points: {} block
// documents which point types are expected
myDaTemp: HpbsDischargeAirTempSensor {
  equipRef: @myAhu
}

mySupplyFan: HpbsSupplyFanRunCmd {
  equipRef: @myAhu
}
```

### Installation

Add to your Haxall project's lib dependencies:

```xeto
depends: {
  { lib: "hpbs", versions: "1.0.x" }
}
```

## Interoperability

All HPBS types remain fully Haystack-compatible:

```axon
// These queries work with HPBS points
read(sensor and air and temp)     // Finds HpbsZoneAirTempSensor
read(boiler)                       // Finds HpbsBoiler
read(chiller)                      // Finds HpbsChiller
read(his and sampled)              // Finds sampled history points
read(vav and hotWaterReheat)       // Finds HpbsVavReheat
```

## Target Platform

- **Haxall**: 4.x
- **Haystack**: 5 (ph 5.0.x)

## References

- **[High Performance Building Standard (HPBS)](https://dfcm.utah.gov/construction-management/high-performance-building-program/)**
- **[HPBS Appendix F - Analytic Points and Tagging Standard](https://dfcm.utah.gov/wp-content/uploads/HPBS-Appendix-F-Analytic-Points-and-Tagging-6-17-19.xlsx)**
- **[Project Haystack](https://project-haystack.org/)** - Industry standard for building data semantics
- **[Haxall Framework](https://github.com/haxall/haxall)** - IoT framework that runs Xeto libraries
- **[Xeto Language](https://github.com/Project-Haystack/xeto)** - Official Xeto specification and standard libraries

## License

Academic Free License version 3.0
