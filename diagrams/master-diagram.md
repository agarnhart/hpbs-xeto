Loaded 1426 specs from 6 libraries

## Class Diagram

```mermaid
classDiagram
    Dict <|-- Lib
    Dict <|-- LibDepend
    Scalar <|-- LibDependVersions
    Dict <|-- LibOrg
    Dict <|-- LibVcs
    Dict <|-- Spec
    Enum <|-- TimeZone
    Obj <|-- Self
    Obj <|-- Scalar
    Scalar <|-- None
    Scalar <|-- Marker
    Scalar <|-- NA
    Scalar <|-- Str
    Scalar <|-- Bool
    Scalar <|-- Number
    Number <|-- Int
    Number <|-- Float
    Number <|-- Duration
    Scalar <|-- Uri
    Scalar <|-- Ref
    Obj <|-- MultiRef
    Scalar <|-- Version
    Scalar <|-- Date
    Scalar <|-- Time
    Scalar <|-- DateTime
    Scalar <|-- Span
    Enum <|-- SpanMode
    Scalar <|-- Enum
    Dict <|-- Choice
    Obj <|-- Seq
    Seq <|-- Dict
    Seq <|-- List
    Seq <|-- Grid
    Obj <|-- Or
    Obj <|-- And
    Scalar <|-- Buf
    Scalar <|-- Filter
    Dict <|-- Query
    Dict <|-- Func
    Interface <|-- Funcs
    Dict <|-- Entity
    Entity <|-- File
    Dict <|-- Interface
    Scalar <|-- BuildVar
    Enum <|-- Unit
    Enum <|-- UnitQuantity
    PhEntity <|-- Attr
    Choice <|-- AhuZoneDelivery
    AhuZoneDelivery <|-- ChilledBeamAhuZoneDelivery
    AhuZoneDelivery <|-- DirectAhuZoneDelivery
    AhuZoneDelivery <|-- MultiAhuZoneDelivery
    AhuZoneDelivery <|-- VavAhuZoneDelivery
    Choice <|-- AirVolumeAdjustability
    AirVolumeAdjustability <|-- ConstantAirVolumeAdjustability
    AirVolumeAdjustability <|-- VariableAirVolumeAdjustability
    Choice <|-- AtesDesign
    AtesDesign <|-- ClosedLoopAtesDesign
    AtesDesign <|-- DoubletAtesDesign
    AtesDesign <|-- DoubletPairedAtesDesign
    AtesDesign <|-- MonoAtesDesign
    AtesDesign <|-- UnidirectionalAtesDesign
    Choice <|-- ChillerMechanism
    ChillerMechanism <|-- AbsorptionChillerMechanism
    ChillerMechanism <|-- CentrifugalChillerMechanism
    ChillerMechanism <|-- ReciprocalChillerMechanism
    ChillerMechanism <|-- RotaryScrewChillerMechanism
    Choice <|-- CondenserLoop
    CondenserLoop <|-- ClosedCondenserLoop
    CondenserLoop <|-- OpenCondenserLoop
    Choice <|-- CoolingProcess
    CoolingProcess <|-- AirCoolingProcess
    CoolingProcess <|-- ChilledWaterCoolingProcess
    CoolingProcess <|-- CondenserCoolingProcess
    CoolingProcess <|-- DxCoolingProcess
    CoolingProcess <|-- WaterCoolingProcess
    Choice <|-- DuctConfig
    DuctConfig <|-- DualDuctConfig
    DuctConfig <|-- SingleDuctConfig
    DuctConfig <|-- TripleDuctConfig
    Choice <|-- DuctDeck
    DuctDeck <|-- ColdDuctDeck
    DuctDeck <|-- HotDuctDeck
    DuctDeck <|-- NeutralDuctDeck
    Choice <|-- DuctSection
    DuctSection <|-- DischargeDuctSection
    DuctSection <|-- EconomizerDuctSection
    DuctSection <|-- ExhaustDuctSection
    DuctSection <|-- FlueDuctSection
    DuctSection <|-- InletDuctSection
    DuctSection <|-- MixedDuctSection
    DuctSection <|-- OutsideDuctSection
    DuctSection <|-- ReturnDuctSection
    DuctSection <|-- VentilationDuctSection
    Choice <|-- HeatingProcess
    HeatingProcess <|-- BiomassHeatingProcess
    HeatingProcess <|-- CoalHeatingProcess
    HeatingProcess <|-- DxHeatingProcess
    HeatingProcess <|-- ElecHeatingProcess
    HeatingProcess <|-- FuelOilHeatingProcess
    HeatingProcess <|-- HotWaterHeatingProcess
    HeatingProcess <|-- NaturalGasHeatingProcess
    HeatingProcess <|-- PropaneHeatingProcess
    HeatingProcess <|-- SteamHeatingProcess
    Choice <|-- MeterScope
    MeterScope <|-- SiteMeterScope
    MeterScope <|-- SubmeterMeterScope
    Choice <|-- PfScope
    PfScope <|-- DisplacementPfScope
    PfScope <|-- DistortionPfScope
    PfScope <|-- TruePfScope
    Choice <|-- PfStandard
    PfStandard <|-- IecPfStandard
    PfStandard <|-- IeeePfStandard
    Choice <|-- PhaseCount
    PhaseCount <|-- SinglePhaseCount
    PhaseCount <|-- SplitPhaseCount
    PhaseCount <|-- ThreePhaseCount
    PhaseCount <|-- TwoPhaseCount
    Choice <|-- PipeSection
    PipeSection <|-- BypassPipeSection
    PipeSection <|-- CircPipeSection
    PipeSection <|-- EnteringPipeSection
    PipeSection <|-- HeaderPipeSection
    PipeSection <|-- LeavingPipeSection
    Choice <|-- PlantLoop
    PlantLoop <|-- PrimaryPlantLoop
    PlantLoop <|-- SecondaryPlantLoop
    PlantLoop <|-- TertiaryPlantLoop
    Choice <|-- PointFunction
    PointFunction <|-- CmdPointFunction
    PointFunction <|-- SensorPointFunction
    PointFunction <|-- SpPointFunction
    PointFunction <|-- SyntheticPointFunction
    SyntheticPointFunction <|-- ComputedSyntheticPointFunction
    SyntheticPointFunction <|-- MlSyntheticPointFunction
    SyntheticPointFunction <|-- SimSyntheticPointFunction
    Choice <|-- SimScenario
    SimScenario <|-- BaselineSimScenario
    SimScenario <|-- OperationSimScenario
    SimScenario <|-- OptimumSimScenario
    Choice <|-- VavAirCircuit
    VavAirCircuit <|-- ParallelVavAirCircuit
    VavAirCircuit <|-- SeriesVavAirCircuit
    Choice <|-- VavModulation
    VavModulation <|-- PressureDependentVavModulation
    VavModulation <|-- PressureIndependentVavModulation
    PhEntity <|-- Device
    PhEntity <|-- Network
    Device <|-- Computer
    Device <|-- Controller
    Phone <|-- MobilePhone
    Device <|-- NetworkingDevice
    NetworkingDevice <|-- NetworkingRouter
    NetworkingDevice <|-- NetworkingSwitch
    Computer <|-- Laptop
    Device <|-- Phone
    Computer <|-- ServerComputer
    Device <|-- Tablet
    Entity <|-- PhEntity
    Enum <|-- CurStatus
    Enum <|-- ElecAcQuadrant
    Enum <|-- EvseCableType
    Enum <|-- GeoCountry
    Enum <|-- GeoState
    Enum <|-- HisMode
    Enum <|-- HisStatus
    Enum <|-- HvacMode
    Enum <|-- Kind
    Enum <|-- Phase
    Enum <|-- PrimaryFunction
    Enum <|-- WeatherCondEnum
    Enum <|-- WeatherDaytimeEnum
    Enum <|-- WriteStatus
    PhEntity <|-- Equip
    ElecMeter <|-- AcElecMeter
    EvsePort <|-- AcEvsePort
    Equip <|-- Actuator
    AirHandlingEquip <|-- Ahu
    Equip <|-- AirHandlingEquip
    Equip <|-- AirTerminalUnit
    Equip <|-- Ates
    Equip <|-- Battery
    Equip <|-- Boiler
    VrfEquip <|-- BranchSelector
    Equip <|-- Cable
    AirTerminalUnit <|-- Cav
    Plant <|-- ChilledWaterPlant
    RadiantEquip <|-- ChilledBeam
    Equip <|-- Chiller
    Equip <|-- Circuit
    HeatExchanger <|-- Coil
    Equip <|-- Conduit
    Panel <|-- ControlsPanel
    Coil <|-- CoolingCoil
    Equip <|-- CoolingTower
    Fcu <|-- Crac
    Actuator <|-- DamperActuator
    ElecMeter <|-- DcElecMeter
    EvsePort <|-- DcEvsePort
    Ahu <|-- Doas
    Conduit <|-- Duct
    Meter <|-- ElecMeter
    Panel <|-- ElecPanel
    VerticalTransport <|-- Elevator
    VerticalTransport <|-- Escalator
    EvseEquip <|-- EvseCable
    EvseEquip <|-- EvseDispenser
    Equip <|-- EvseEquip
    EvseEquip <|-- EvsePort
    EvseEquip <|-- EvsePowerConverter
    Motor <|-- FanMotor
    AirHandlingEquip <|-- Fcu
    Meter <|-- FlowMeter
    Equip <|-- FlowInverter
    Equip <|-- FumeHood
    Equip <|-- HeatExchanger
    Coil <|-- HeatingCoil
    Boiler <|-- HotWaterBoiler
    Plant <|-- HotWaterPlant
    Equip <|-- HumidifierEquip
    Equip <|-- Luminaire
    Doas <|-- Mau
    Equip <|-- Meter
    Equip <|-- Motor
    VerticalTransport <|-- MovingWalkway
    Equip <|-- Panel
    Conduit <|-- Pipe
    Equip <|-- Plant
    Motor <|-- PumpMotor
    Equip <|-- Rack
    Equip <|-- RadiantEquip
    RadiantEquip <|-- RadiantFloor
    RadiantEquip <|-- Radiator
    Ahu <|-- Rtu
    Boiler <|-- SteamBoiler
    Plant <|-- SteamPlant
    Equip <|-- Tank
    Equip <|-- Thermostat
    Fcu <|-- UnitVent
    Equip <|-- Ups
    Actuator <|-- ValveActuator
    AirTerminalUnit <|-- Vav
    Equip <|-- VerticalTransport
    Equip <|-- VrfEquip
    VrfEquip <|-- VrfIndoorUnit
    VrfIndoorUnit <|-- VrfIndoorUnitFcu
    VrfEquip <|-- VrfOutdoorUnit
    Plant <|-- VrfRefrigPlant
    Equip <|-- Well
    Conduit <|-- Wire
    Feature <|-- Filetype
    Scalar <|-- Symbol
    Scalar <|-- Coord
    Scalar <|-- XStr
    Dict <|-- Feature
    Feature <|-- Op
    Choice <|-- Phenomenon
    Phenomenon <|-- Elec
    Elec <|-- AcElec
    Elec <|-- DcElec
    Phenomenon <|-- Light
    Phenomenon <|-- Solar
    Phenomenon <|-- Substance
    Substance <|-- Biomass
    Substance <|-- Fluid
    Fluid <|-- Gas
    Gas <|-- Air
    Gas <|-- Ch2o
    Gas <|-- Ch4
    Gas <|-- Co
    Gas <|-- Co2
    Gas <|-- Hfc
    Gas <|-- N2o
    Gas <|-- NaturalGas
    Gas <|-- Nf3
    Gas <|-- Nh3
    Gas <|-- No2
    Gas <|-- O2
    Gas <|-- O3
    Gas <|-- Pfc
    Gas <|-- Propane
    Gas <|-- Sf6
    Gas <|-- Steam
    Gas <|-- Tvoc
    Fluid <|-- Liquid
    Liquid <|-- Condensate
    Liquid <|-- Diesel
    Liquid <|-- FuelOil
    Liquid <|-- Gasoline
    Liquid <|-- Water
    Water <|-- BlowdownWater
    Water <|-- ChilledWater
    Water <|-- ColdWater
    Water <|-- CondenserWater
    Water <|-- CoolWater
    Water <|-- DomesticWater
    Water <|-- GroundWater
    Water <|-- HotWater
    Water <|-- MakeupWater
    Water <|-- PurgeWater
    Water <|-- WarmWater
    Fluid <|-- Refrig
    Substance <|-- Solid
    Solid <|-- Coal
    Solid <|-- Ice
    Solid <|-- Pm01
    Solid <|-- Pm10
    Solid <|-- Pm25
    Phenomenon <|-- Weather
    Phenomenon <|-- Wind
    PhEntity <|-- Point
    Point <|-- CurPoint
    Point <|-- HisPoint
    Point <|-- WritablePoint
    Point <|-- SyntheticPoint
    PhEntity <|-- SyntheticModel
    SyntheticPoint <|-- ComputedPoint
    SyntheticModel <|-- ComputedModel
    SyntheticPoint <|-- MlPoint
    SyntheticModel <|-- MlModel
    PhEntity <|-- MlVar
    SyntheticPoint <|-- SimPoint
    SyntheticModel <|-- SimModel
    Choice <|-- Quantity
    Quantity <|-- AirVelocity
    Quantity <|-- ApparentEnergy
    Quantity <|-- ApparentPower
    Quantity <|-- Cloudage
    Quantity <|-- Concentration
    Concentration <|-- AirQuality
    AirQuality <|-- Ch2oConcentration
    AirQuality <|-- CoConcentration
    AirQuality <|-- Co2Concentration
    AirQuality <|-- Nh3Concentration
    AirQuality <|-- No2Concentration
    AirQuality <|-- O3Concentration
    AirQuality <|-- Pm01Concentration
    AirQuality <|-- Pm10Concentration
    AirQuality <|-- Pm25Concentration
    AirQuality <|-- TvocConcentration
    Quantity <|-- CurrentAngle
    Quantity <|-- CurrentImbalance
    Quantity <|-- CurrentThd
    Quantity <|-- Daytime
    Quantity <|-- DewPoint
    Quantity <|-- Direction
    Direction <|-- WindDirection
    Quantity <|-- ElecCurrent
    ElecCurrent <|-- CurrentMagnitude
    Quantity <|-- ElecVolt
    ElecVolt <|-- VoltMagnitude
    Quantity <|-- Emission
    Emission <|-- Ch4Emission
    Emission <|-- Co2Emission
    Emission <|-- HfcEmission
    Emission <|-- N2oEmission
    Emission <|-- Nf3Emission
    Emission <|-- PfcEmission
    Emission <|-- Sf6Emission
    Quantity <|-- Energy
    Energy <|-- ElecEnergy
    ElecEnergy <|-- ActiveEnergy
    Quantity <|-- Enthalpy
    Quantity <|-- FeelsLike
    Quantity <|-- Flow
    Quantity <|-- Freq
    Freq <|-- AcFreq
    Quantity <|-- Humidity
    Quantity <|-- Illuminance
    Quantity <|-- Irradiance
    Irradiance <|-- SolarIrradiance
    Quantity <|-- Level
    Level <|-- LightLevel
    Quantity <|-- Luminance
    Quantity <|-- LuminousFlux
    Quantity <|-- LuminousIntensity
    Quantity <|-- Pf
    Quantity <|-- Power
    Power <|-- ElecPower
    ElecPower <|-- ActivePower
    ActivePower <|-- ElecDemand
    Quantity <|-- Precipitation
    Quantity <|-- Pressure
    Pressure <|-- AtmosphericPressure
    Quantity <|-- ReactiveEnergy
    Quantity <|-- ReactivePower
    Quantity <|-- Speed
    Speed <|-- WindSpeed
    Quantity <|-- StateOfCharge
    Quantity <|-- Temp
    Temp <|-- AirTemp
    Quantity <|-- VfdFreq
    Quantity <|-- VfdSpeed
    Quantity <|-- Visibility
    Quantity <|-- VoltAngle
    Quantity <|-- VoltImbalance
    Quantity <|-- VoltThd
    Quantity <|-- Volume
    Quantity <|-- WeatherCond
    Quantity <|-- WetBulb
    GeoPlace <|-- Site
    PhEntity <|-- GeoPlace
    PhEntity <|-- Space
    Space <|-- DataCenter
    Space <|-- Floor
    Floor <|-- GroundFloor
    ZoneSpace <|-- HvacZoneSpace
    ZoneSpace <|-- LightingZoneSpace
    Floor <|-- RoofFloor
    Space <|-- Room
    Floor <|-- SubterraneanFloor
    Space <|-- ZoneSpace
    PhEntity <|-- System
    System <|-- AirSystem
    AirSystem <|-- AirConditioningSystem
    AirSystem <|-- AirExhaustSystem
    AirSystem <|-- AirVentilationSystem
    System <|-- WaterSystem
    WaterSystem <|-- ChilledWaterSystem
    WaterSystem <|-- CondenserWaterSystem
    DomesticWaterSystem <|-- DomesticColdWaterSystem
    DomesticWaterSystem <|-- DomesticHotWaterSystem
    WaterSystem <|-- DomesticWaterSystem
    WaterSystem <|-- HotWaterSystem
    WaterSystem <|-- SteamSystem
    System <|-- ElecSystem
    ElecSystem <|-- EvseSystem
    ElecSystem <|-- LightingSystem
    System <|-- RefrigSystem
    RefrigSystem <|-- VrfSystem
    VrfSystem <|-- VrfCoolingOnlySystem
    VrfSystem <|-- VrfHeatPumpSystem
    VrfSystem <|-- VrfHeatRecoverySystem
    GeoPlace <|-- WeatherStation
    Point <|-- WeatherPoint
    NumberPoint <|-- AirFlowPoint
    AirFlowPoint <|-- AirFlowSensor
    AirFlowPoint <|-- AirFlowSp
    AirFlowSensor <|-- DischargeAirFlowSensor
    AirFlowSp <|-- DischargeAirFlowSp
    DischargeAirFlowSensor <|-- ColdDeckDischargeAirFlowSensor
    DischargeAirFlowSp <|-- ColdDeckDischargeAirFlowSp
    DischargeAirFlowSensor <|-- HotDeckDischargeAirFlowSensor
    DischargeAirFlowSp <|-- HotDeckDischargeAirFlowSp
    AirFlowSensor <|-- EconomizingAirFlowSensor
    AirFlowSp <|-- EconomizingAirFlowSp
    AirFlowSensor <|-- ExhaustAirFlowSensor
    AirFlowSp <|-- ExhaustAirFlowSp
    AirFlowSensor <|-- InletAirFlowSensor
    AirFlowSp <|-- InletAirFlowSp
    AirFlowSensor <|-- OutsideAirFlowSensor
    AirFlowSp <|-- OutsideAirFlowSp
    AirFlowSensor <|-- ReturnAirFlowSensor
    AirFlowSp <|-- ReturnAirFlowSp
    AirFlowSensor <|-- VentilationAirFlowSensor
    AirFlowSp <|-- VentilationAirFlowSp
    NumberPoint <|-- AirHumidityPoint
    AirHumidityPoint <|-- AirHumiditySensor
    AirHumidityPoint <|-- AirHumiditySp
    AirHumiditySensor <|-- DischargeAirHumiditySensor
    AirHumiditySp <|-- DischargeAirHumiditySp
    AirHumiditySensor <|-- OutdoorAirHumiditySensor
    AirHumiditySp <|-- OutdoorAirHumiditySp
    AirHumiditySensor <|-- ZoneAirHumiditySensor
    AirHumiditySp <|-- ZoneAirHumiditySp
    NumberPoint <|-- AirPressurePoint
    AirPressurePoint <|-- AirPressureSensor
    AirPressurePoint <|-- AirPressureSp
    AirPressureSensor <|-- DischargeAirPressureSensor
    AirPressureSp <|-- DischargeAirPressureSp
    AirPressureSensor <|-- ReturnAirPressureSensor
    AirPressureSp <|-- ReturnAirPressureSp
    NumberPoint <|-- AirTempPoint
    AirTempPoint <|-- AirTempSensor
    AirTempPoint <|-- AirTempSp
    AirTempSensor <|-- DischargeAirTempSensor
    AirTempSp <|-- DischargeAirTempSp
    AirTempSensor <|-- EconomizingAirTempSensor
    AirTempSensor <|-- InletAirTempSensor
    AirTempSp <|-- InletAirTempSp
    AirTempSensor <|-- MixedAirTempSensor
    AirTempSp <|-- MixedAirTempSp
    AirTempSensor <|-- OutsideAirTempSensor
    AirTempSensor <|-- ReturnAirTempSensor
    AirTempSp <|-- ReturnAirTempSp
    AirTempSensor <|-- VentilationAirTempSensor
    AirTempSensor <|-- ZoneAirTempSensor
    AirTempSp <|-- ZoneAirTempSp
    ZoneAirTempSp <|-- ZoneAirTempEffectiveSp
    ZoneAirTempSp <|-- ZoneAirTempCoolingSp
    ZoneAirTempCoolingSp <|-- ZoneAirTempOccCoolingSp
    ZoneAirTempCoolingSp <|-- ZoneAirTempUnoccCoolingSp
    ZoneAirTempCoolingSp <|-- ZoneAirTempStandbyCoolingSp
    ZoneAirTempSp <|-- ZoneAirTempHeatingSp
    ZoneAirTempHeatingSp <|-- ZoneAirTempOccHeatingSp
    ZoneAirTempHeatingSp <|-- ZoneAirTempUnoccHeatingSp
    ZoneAirTempHeatingSp <|-- ZoneAirTempStandbyHeatingSp
    Point <|-- BoolPoint
    Point <|-- NumberPoint
    Point <|-- EnumPoint
    Point <|-- CmdPoint
    Point <|-- SensorPoint
    Point <|-- SpPoint
    SyntheticPoint <|-- ComputedSyntheticPoint
    SyntheticPoint <|-- MlSyntheticPoint
    SyntheticPoint <|-- SimSyntheticPoint
    NumberPoint <|-- Co2Point
    Co2Point <|-- Co2Sensor
    Co2Point <|-- Co2Sp
    Co2Sensor <|-- ZoneCo2Sensor
    Co2Sp <|-- ZoneCo2Sp
    NumberPoint <|-- DamperPoint
    DamperPoint <|-- DamperSensor
    DamperPoint <|-- DamperCmd
    DamperSensor <|-- DischargeDamperSensor
    DamperCmd <|-- DischargeDamperCmd
    DischargeDamperSensor <|-- ColdDeckDischargeDamperSensor
    DischargeDamperCmd <|-- ColdDeckDischargeDamperCmd
    DischargeDamperSensor <|-- HotDeckDischargeDamperSensor
    DischargeDamperCmd <|-- HotDeckDischargeDamperCmd
    DamperSensor <|-- EconomizingDamperSensor
    DamperCmd <|-- EconomizingDamperCmd
    DamperSensor <|-- ExhaustDamperSensor
    DamperCmd <|-- ExhaustDamperCmd
    DamperSensor <|-- MixedDamperSensor
    DamperCmd <|-- MixedDamperCmd
    DamperSensor <|-- OutsideDamperSensor
    DamperCmd <|-- OutsideDamperCmd
    DamperSensor <|-- ReturnDamperSensor
    DamperCmd <|-- ReturnDamperCmd
    DamperSensor <|-- VentilationDamperSensor
    DamperCmd <|-- VentilationDamperCmd
    Choice <|-- ElecDirection
    ElecDirection <|-- ElecImportDirection
    ElecDirection <|-- ElecExportDirection
    ElecDirection <|-- ElecNetDirection
    ElecDirection <|-- ElecAbsoluteDirection
    Choice <|-- ElecAcPowerSubtype
    ElecAcPowerSubtype <|-- ElecAcActivePower
    ElecAcPowerSubtype <|-- ElecAcReactivePower
    ElecAcPowerSubtype <|-- ElecAcApparentPower
    NumberPoint <|-- ElecSensor
    ElecSensor <|-- ElecDemandSensor
    ElecSensor <|-- ElecEnergySensor
    ElecSensor <|-- ElecAcPfSensor
    ElecEnergySensor <|-- ElecAcEnergySensor
    ElecAcEnergySensor <|-- ElecAcActiveEnergySensor
    ElecAcEnergySensor <|-- ElecAcReactiveEnergySensor
    ElecAcEnergySensor <|-- ElecAcApparentEnergySensor
    ElecDemandSensor <|-- ElecAcDemandSensor
    ElecAcDemandSensor <|-- ElecAcPowerDemandSensor
    ElecAcPowerDemandSensor <|-- ElecAcActiveDemandSensor
    ElecAcPowerDemandSensor <|-- ElecAcReactiveDemandSensor
    ElecAcPowerDemandSensor <|-- ElecAcApparentDemandSensor
    ElecAcActiveEnergySensor <|-- ElecAcImportActiveEnergySensor
    ElecAcActiveEnergySensor <|-- ElecAcExportActiveEnergySensor
    ElecAcActiveEnergySensor <|-- ElecAcNetActiveEnergySensor
    ElecAcReactiveEnergySensor <|-- ElecAcImportReactiveEnergySensor
    ElecAcReactiveEnergySensor <|-- ElecAcExportReactiveEnergySensor
    ElecAcReactiveEnergySensor <|-- ElecAcNetReactiveEnergySensor
    ElecAcApparentEnergySensor <|-- ElecAcImportApparentEnergySensor
    ElecAcApparentEnergySensor <|-- ElecAcExportApparentEnergySensor
    ElecAcApparentEnergySensor <|-- ElecAcNetApparentEnergySensor
    ElecAcActiveDemandSensor <|-- ElecAcImportActiveDemandSensor
    ElecAcActiveDemandSensor <|-- ElecAcExportActiveDemandSensor
    ElecAcActiveDemandSensor <|-- ElecAcNetActiveDemandSensor
    ElecAcReactiveDemandSensor <|-- ElecAcImportReactiveDemandSensor
    ElecAcReactiveDemandSensor <|-- ElecAcExportReactiveDemandSensor
    ElecAcReactiveDemandSensor <|-- ElecAcNetReactiveDemandSensor
    ElecAcApparentDemandSensor <|-- ElecAcImportApparentDemandSensor
    ElecAcApparentDemandSensor <|-- ElecAcExportApparentDemandSensor
    ElecAcApparentDemandSensor <|-- ElecAcNetApparentDemandSensor
    ElecAcImportActiveEnergySensor <|-- ElecAcTotalImportActiveEnergySensor
    ElecAcExportActiveEnergySensor <|-- ElecAcTotalExportActiveEnergySensor
    ElecAcNetActiveEnergySensor <|-- ElecAcTotalNetActiveEnergySensor
    ElecAcImportReactiveEnergySensor <|-- ElecAcTotalImportReactiveEnergySensor
    ElecAcExportReactiveEnergySensor <|-- ElecAcTotalExportReactiveEnergySensor
    ElecAcNetReactiveEnergySensor <|-- ElecAcTotalNetReactiveEnergySensor
    ElecAcImportApparentEnergySensor <|-- ElecAcTotalImportApparentEnergySensor
    ElecAcExportApparentEnergySensor <|-- ElecAcTotalExportApparentEnergySensor
    ElecAcNetApparentEnergySensor <|-- ElecAcTotalNetApparentEnergySensor
    ElecAcPfSensor <|-- ElecAcTotalPfSensor
    ElecAcImportActiveDemandSensor <|-- ElecAcTotalImportActiveDemandSensor
    ElecAcExportActiveDemandSensor <|-- ElecAcTotalExportActiveDemandSensor
    ElecAcNetActiveDemandSensor <|-- ElecAcTotalNetActiveDemandSensor
    ElecAcImportReactiveDemandSensor <|-- ElecAcTotalImportReactiveDemandSensor
    ElecAcExportReactiveDemandSensor <|-- ElecAcTotalExportReactiveDemandSensor
    ElecAcNetReactiveDemandSensor <|-- ElecAcTotalNetReactiveDemandSensor
    ElecAcImportApparentDemandSensor <|-- ElecAcTotalImportApparentDemandSensor
    ElecAcExportApparentDemandSensor <|-- ElecAcTotalExportApparentDemandSensor
    ElecAcNetApparentDemandSensor <|-- ElecAcTotalNetApparentDemandSensor
    Point <|-- FanPoint
    FanPoint <|-- FanRunSensor
    FanPoint <|-- FanRunCmd
    FanPoint <|-- FanEnableSensor
    FanPoint <|-- FanEnableCmd
    FanPoint <|-- FanSpeedSensor
    FanPoint <|-- FanSpeedCmd
    FanRunSensor <|-- DischargeFanRunSensor
    FanRunCmd <|-- DischargeFanRunCmd
    FanEnableSensor <|-- DischargeFanEnableSensor
    FanEnableCmd <|-- DischargeFanEnableCmd
    FanSpeedSensor <|-- DischargeFanSpeedSensor
    FanSpeedCmd <|-- DischargeFanSpeedCmd
    FanRunSensor <|-- ReturnFanRunSensor
    FanRunCmd <|-- ReturnFanRunCmd
    FanEnableSensor <|-- ReturnFanEnableSensor
    FanEnableCmd <|-- ReturnFanEnableCmd
    FanSpeedSensor <|-- ReturnFanSpeedSensor
    FanSpeedCmd <|-- ReturnFanSpeedCmd
    BoolPoint <|-- CoolCmd
    BoolPoint <|-- HeatCmd
    BoolPoint <|-- DessicantDehumidifierCmd
    EnumPoint <|-- ZoneAirHvacModeSp
    BoolPoint <|-- RunPoint
    Enum <|-- RunEnum
    RunPoint <|-- RunSensor
    RunPoint <|-- RunCmd
    BoolPoint <|-- EnablePoint
    EnablePoint <|-- EnableSensor
    EnablePoint <|-- EnableCmd
    BoolPoint <|-- AlarmSensor
    NumberPoint <|-- VfdFreqPoint
    VfdFreqPoint <|-- VfdFreqSensor
    VfdFreqPoint <|-- VfdFreqCmd
    NumberPoint <|-- VfdSpeedPoint
    VfdSpeedPoint <|-- VfdSpeedSensor
    VfdSpeedPoint <|-- VfdSpeedCmd
    NumberPoint <|-- NaturalGasFlowPoint
    NaturalGasFlowPoint <|-- NaturalGasFlowSensor
    NaturalGasFlowPoint <|-- NaturalGasFlowSp
    NumberPoint <|-- NaturalGasVolumePoint
    NaturalGasVolumePoint <|-- NaturalGasVolumeSensor
    NaturalGasVolumePoint <|-- NaturalGasVolumeSp
    NumberPoint <|-- NaturalGasEnergyPoint
    NaturalGasEnergyPoint <|-- NaturalGasEnergySensor
    NaturalGasEnergyPoint <|-- NaturalGasEnergySp
    BoolPoint <|-- OccupiedPoint
    Enum <|-- OccupiedEnum
    OccupiedPoint <|-- OccupiedSensor
    OccupiedPoint <|-- OccupiedSp
    OccupiedSensor <|-- ZoneOccupiedSensor
    OccupiedSp <|-- ZoneOccupiedSp
    NumberPoint <|-- ValvePoint
    ValvePoint <|-- ValveSensor
    ValvePoint <|-- ValveCmd
    ValveSensor <|-- ChilledWaterValveSensor
    ValveCmd <|-- ChilledWaterValveCmd
    ValveSensor <|-- HotWaterValveSensor
    ValveCmd <|-- HotWaterValveCmd
    NumberPoint <|-- WaterFlowPoint
    WaterFlowPoint <|-- WaterFlowSensor
    WaterFlowPoint <|-- WaterFlowSp
    WaterFlowSensor <|-- DomesticWaterFlowSensor
    WaterFlowSp <|-- DomesticWaterFlowSp
    WaterFlowSensor <|-- ChilledWaterFlowSensor
    WaterFlowSp <|-- ChilledWaterFlowSp
    WaterFlowSensor <|-- HotWaterFlowSensor
    WaterFlowSp <|-- HotWaterFlowSp
    NumberPoint <|-- WaterPressurePoint
    WaterPressurePoint <|-- WaterPressureSensor
    WaterPressurePoint <|-- WaterPressureSp
    WaterPressureSensor <|-- ChilledWaterLeavingPressureSensor
    WaterPressureSensor <|-- ChilledWaterEnteringPressureSensor
    WaterPressureSp <|-- ChilledWaterLeavingPressureSp
    WaterPressureSp <|-- ChilledWaterEnteringPressureSp
    WaterPressureSensor <|-- HotWaterLeavingPressureSensor
    WaterPressureSensor <|-- HotWaterEnteringPressureSensor
    WaterPressureSp <|-- HotWaterLeavingPressureSp
    WaterPressureSp <|-- HotWaterEnteringPressureSp
    NumberPoint <|-- WaterTempPoint
    WaterTempPoint <|-- WaterTempSensor
    WaterTempPoint <|-- WaterTempSp
    WaterTempSensor <|-- HotWaterEnteringTempSensor
    WaterTempSensor <|-- HotWaterLeavingTempSensor
    WaterTempSp <|-- HotWaterLeavingTempSp
    WaterTempSensor <|-- ChilledWaterEnteringTempSensor
    WaterTempSensor <|-- ChilledWaterLeavingTempSensor
    WaterTempSp <|-- ChilledWaterLeavingTempSp
    WaterTempSensor <|-- CondenserWaterEnteringTempSensor
    WaterTempSensor <|-- CondenserWaterLeavingTempSensor
    WaterTempSp <|-- CondenserWaterLeavingTempSp
    NumberPoint <|-- WaterVolumePoint
    WaterVolumePoint <|-- WaterVolumeSensor
    WaterVolumePoint <|-- WaterVolumeSp
    WaterVolumeSensor <|-- DomesticWaterVolumeSensor
    WaterVolumeSp <|-- DomesticWaterVolumeSp
    WeatherPoint <|-- WeatherCondPoint
    WeatherPoint <|-- WeatherDaytimePoint
    WeatherPoint <|-- WeatherNumberPoint
    WeatherNumberPoint <|-- WeatherTempPoint
    WeatherNumberPoint <|-- WeatherWetbulbPoint
    WeatherNumberPoint <|-- WeatherFeelsLikePoint
    WeatherNumberPoint <|-- WeatherDewPointPoint
    WeatherNumberPoint <|-- WeatherHumidityPoint
    WeatherNumberPoint <|-- WeatherEnthalpyPoint
    WeatherNumberPoint <|-- WeatherAtmosphericPressurePoint
    WeatherNumberPoint <|-- WeatherCloudagePoint
    WeatherNumberPoint <|-- WeatherPrecipitationPoint
    WeatherNumberPoint <|-- WeatherSolarIrradiancePoint
    WeatherNumberPoint <|-- WeatherWindSpeedPoint
    WeatherNumberPoint <|-- WeatherWindDirectionPoint
    WeatherNumberPoint <|-- WeatherVisibilityPoint
    Choice <|-- ElecDemandCalc
    ElecDemandCalc <|-- ElecFixedWindowDemandCalc
    ElecDemandCalc <|-- ElecSlidingWindowDemandCalc
    Choice <|-- ElecAcSpectralContent
    ElecAcSpectralContent <|-- ElecAcWaveform
    ElecAcSpectralContent <|-- ElecAcFundamentalComponent
    ElecAcSpectralContent <|-- ElecAcHarmonicComponent
    Choice <|-- ElecAcWaveformMagnitude
    ElecAcWaveformMagnitude <|-- ElecAcAvgWaveformMagnitude
    ElecAcWaveformMagnitude <|-- ElecAcRmsWaveformMagnitude
    ElecAcWaveformMagnitude <|-- ElecAcPeakWaveformMagnitude
    ElecAcWaveformMagnitude <|-- ElecAcPeakToPeakWaveformMagnitude
    Choice <|-- ElecAcQualityMetric
    ElecAcQualityMetric <|-- ElecAcThffQualityMetric
    ElecAcQualityMetric <|-- ElecAcIhdQualityMetric
    ElecAcQualityMetric <|-- ElecAcThdQualityMetric
    ElecAcQualityMetric <|-- ElecAcOddThdQualityMetric
    ElecAcQualityMetric <|-- ElecAcEvenThdQualityMetric
    ElecAcQualityMetric <|-- ElecAcKFactorQualityMetric
    ElecAcQualityMetric <|-- ElecAcCrestFactorQualityMetric
    ElecAcQualityMetric <|-- ElecAcImbalanceQualityMetric
    ElecVoltSensor <|-- ElecDcVoltSensor
    ElecCurrentSensor <|-- ElecDcCurrentSensor
    ElecPowerSensor <|-- ElecDcPowerSensor
    ElecEnergySensor <|-- ElecDcEnergySensor
    ElecSensor <|-- ElecDcStateOfChargeSensor
    ElecDcPowerSensor <|-- ElecDcImportPowerSensor
    ElecDcPowerSensor <|-- ElecDcExportPowerSensor
    ElecDcPowerSensor <|-- ElecDcNetPowerSensor
    ElecDcCurrentSensor <|-- ElecDcImportCurrentSensor
    ElecDcCurrentSensor <|-- ElecDcExportCurrentSensor
    ElecDcCurrentSensor <|-- ElecDcNetCurrentSensor
    ElecDcEnergySensor <|-- ElecDcImportEnergySensor
    ElecDcEnergySensor <|-- ElecDcExportEnergySensor
    ElecDcEnergySensor <|-- ElecDcNetEnergySensor
    ElecSensor <|-- ElecVoltSensor
    ElecSensor <|-- ElecCurrentSensor
    ElecSensor <|-- ElecPowerSensor
    ElecSensor <|-- ElecAcFreqSensor
    ElecVoltSensor <|-- ElecAcVoltSensorX
    ElecAcVoltSensorX <|-- ElecAcMagnitudeVoltSensor
    ElecAcMagnitudeVoltSensor <|-- ElecAcVoltSensor
    ElecAcVoltSensorX <|-- ElecAcAngleVoltSensor
    ElecAcVoltSensorX <|-- ElecAcQualityVoltSensor
    ElecCurrentSensor <|-- ElecAcCurrentSensorX
    ElecAcCurrentSensorX <|-- ElecAcMagnitudeCurrentSensor
    ElecAcMagnitudeCurrentSensor <|-- ElecAcCurrentSensor
    ElecAcCurrentSensorX <|-- ElecAcAngleCurrentSensor
    ElecAcCurrentSensorX <|-- ElecAcQualityCurrentSensor
    ElecAcDemandSensor <|-- ElecAcCurrentDemandSensor
    ElecPowerSensor <|-- ElecAcAvgMagnitudePowerSensor
    ElecAcAvgMagnitudePowerSensor <|-- ElecAcActivePowerSensor
    ElecAcAvgMagnitudePowerSensor <|-- ElecAcReactivePowerSensor
    ElecAcAvgMagnitudePowerSensor <|-- ElecAcApparentPowerSensor
    ElecAcActivePowerSensor <|-- ElecAcImportActivePowerSensor
    ElecAcActivePowerSensor <|-- ElecAcExportActivePowerSensor
    ElecAcActivePowerSensor <|-- ElecAcNetActivePowerSensor
    ElecAcReactivePowerSensor <|-- ElecAcImportReactivePowerSensor
    ElecAcReactivePowerSensor <|-- ElecAcExportReactivePowerSensor
    ElecAcReactivePowerSensor <|-- ElecAcNetReactivePowerSensor
    ElecAcApparentPowerSensor <|-- ElecAcImportApparentPowerSensor
    ElecAcApparentPowerSensor <|-- ElecAcExportApparentPowerSensor
    ElecAcApparentPowerSensor <|-- ElecAcNetApparentPowerSensor
    ElecAcCurrentDemandSensor <|-- ElecAcNetCurrentDemandSensor
    ElecAcVoltSensor <|-- ElecAcLLAvgVoltSensor
    ElecAcVoltSensor <|-- ElecAcPhaseVoltSensor
    ElecAcVoltSensor <|-- ElecAcLAvgVoltSensor
    ElecAcAngleVoltSensor <|-- ElecAcPhaseAngleVoltSensor
    ElecAcQualityVoltSensor <|-- ElecAcLLAvgQualityVoltSensor
    ElecAcQualityVoltSensor <|-- ElecAcPhaseQualityVoltSensor
    ElecAcQualityVoltSensor <|-- ElecAcLAvgQualityVoltSensor
    ElecAcCurrentSensor <|-- ElecAcLAvgCurrentSensor
    ElecAcCurrentSensor <|-- ElecAcPhaseCurrentSensor
    ElecAcCurrentSensor <|-- ElecAcNeutralCurrentSensor
    ElecAcCurrentSensor <|-- ElecAcGroundCurrentSensor
    ElecAcAngleCurrentSensor <|-- ElecAcPhaseAngleCurrentSensor
    ElecAcAngleCurrentSensor <|-- ElecAcNeutralAngleCurrentSensor
    ElecAcAngleCurrentSensor <|-- ElecAcGroundAngleCurrentSensor
    ElecAcQualityCurrentSensor <|-- ElecAcPhaseQualityCurrentSensor
    ElecAcQualityCurrentSensor <|-- ElecAcLAvgQualityCurrentSensor
    ElecAcQualityCurrentSensor <|-- ElecAcNeutralQualityCurrentSensor
    ElecAcQualityCurrentSensor <|-- ElecAcGroundQualityCurrentSensor
    ElecAcNetCurrentDemandSensor <|-- ElecAcPhaseNetCurrentDemandSensor
    ElecAcImportActivePowerSensor <|-- ElecAcTotalImportActivePowerSensor
    ElecAcExportActivePowerSensor <|-- ElecAcTotalExportActivePowerSensor
    ElecAcNetActivePowerSensor <|-- ElecAcTotalNetActivePowerSensor
    ElecAcImportActivePowerSensor <|-- ElecAcPhaseImportActivePowerSensor
    ElecAcExportActivePowerSensor <|-- ElecAcPhaseExportActivePowerSensor
    ElecAcNetActivePowerSensor <|-- ElecAcPhaseNetActivePowerSensor
    ElecAcImportReactivePowerSensor <|-- ElecAcTotalImportReactivePowerSensor
    ElecAcExportReactivePowerSensor <|-- ElecAcTotalExportReactivePowerSensor
    ElecAcNetReactivePowerSensor <|-- ElecAcTotalNetReactivePowerSensor
    ElecAcImportReactivePowerSensor <|-- ElecAcPhaseImportReactivePowerSensor
    ElecAcExportReactivePowerSensor <|-- ElecAcPhaseExportReactivePowerSensor
    ElecAcNetReactivePowerSensor <|-- ElecAcPhaseNetReactivePowerSensor
    ElecAcImportApparentPowerSensor <|-- ElecAcTotalImportApparentPowerSensor
    ElecAcExportApparentPowerSensor <|-- ElecAcTotalExportApparentPowerSensor
    ElecAcNetApparentPowerSensor <|-- ElecAcTotalNetApparentPowerSensor
    ElecAcImportApparentPowerSensor <|-- ElecAcPhaseImportApparentPowerSensor
    ElecAcExportApparentPowerSensor <|-- ElecAcPhaseExportApparentPowerSensor
    ElecAcNetApparentPowerSensor <|-- ElecAcPhaseNetApparentPowerSensor
    ElecAcPfSensor <|-- ElecAcPhasePfSensor
    ElecAcImportActiveEnergySensor <|-- ElecAcPhaseImportActiveEnergySensor
    ElecAcExportActiveEnergySensor <|-- ElecAcPhaseExportActiveEnergySensor
    ElecAcNetActiveEnergySensor <|-- ElecAcPhaseNetActiveEnergySensor
    ElecAcImportReactiveEnergySensor <|-- ElecAcPhaseImportReactiveEnergySensor
    ElecAcExportReactiveEnergySensor <|-- ElecAcPhaseExportReactiveEnergySensor
    ElecAcNetReactiveEnergySensor <|-- ElecAcPhaseNetReactiveEnergySensor
    ElecAcImportApparentEnergySensor <|-- ElecAcPhaseImportApparentEnergySensor
    ElecAcExportApparentEnergySensor <|-- ElecAcPhaseExportApparentEnergySensor
    ElecAcNetApparentEnergySensor <|-- ElecAcPhaseNetApparentEnergySensor
    ElecCurrentMaxSp <|-- ElecDcCurrentMaxSp
    ElecPowerMaxSp <|-- ElecDcPowerMaxSp
    ElecDcPowerMaxSp <|-- ElecDcImportPowerMaxSp
    ElecDcCurrentMaxSp <|-- ElecDcImportCurrentMaxSp
    NumberPoint <|-- ElecSp
    ElecSp <|-- ElecMaxSp
    ElecMaxSp <|-- ElecCurrentMaxSp
    ElecMaxSp <|-- ElecPowerMaxSp
    ElecMaxSp <|-- ElecDemandMaxSp
    ElecCurrentMaxSp <|-- ElecAcCurrentMaxSp
    ElecPowerMaxSp <|-- ElecAcPowerMaxSp
    ElecAcPowerMaxSp <|-- ElecAcMagnitudePowerMaxSp
    ElecAcMagnitudePowerMaxSp <|-- ElecAcActivePowerMaxSp
    ElecDemandMaxSp <|-- ElecAcActiveDemandMaxSp
    ElecAcCurrentMaxSp <|-- ElecAcImportCurrentMaxSp
    ElecAcActivePowerMaxSp <|-- ElecAcImportActivePowerMaxSp
    ElecAcActiveDemandMaxSp <|-- ElecAcImportActiveDemandMaxSp
    ElecAcImportCurrentMaxSp <|-- ElecAcPhaseImportCurrentMaxSp
    ElecAcImportActivePowerMaxSp <|-- ElecAcTotalImportActivePowerMaxSp
    ElecAcImportActiveDemandMaxSp <|-- ElecAcTotalImportActiveDemandMaxSp
    Duct <|-- EconomizerDuct
    Duct <|-- FlueDuct
    Duct <|-- InletDuct
    Duct <|-- VentilationDuct
    Duct <|-- OutsideDuct
    Duct <|-- DischargeDuct
    Duct <|-- ExhaustDuct
    Duct <|-- ReturnDuct
    DuctSection <|-- MixedDuct
    DischargeDuct <|-- ColdDeckDischargeDuct
    DischargeDuct <|-- HotDeckDischargeDuct
    DischargeDuct <|-- NeutralDeckDischargeDuct
    Ahu <|-- VavZoneAhu
    Vav <|-- AhuVav
    FlowMeter <|-- WaterMeter
    WaterMeter <|-- DomesticWaterMeter
    FlowMeter <|-- NaturalGasMeter
    ZoneAirTempSensor <|-- HpbsZoneAirTempSensor
    ZoneAirTempEffectiveSp <|-- HpbsZoneAirTempEffectiveSp
    ZoneAirTempCoolingSp <|-- HpbsZoneAirTempCoolingSp
    ZoneAirTempHeatingSp <|-- HpbsZoneAirTempHeatingSp
    ZoneAirTempOccCoolingSp <|-- HpbsZoneAirTempOccCoolingSp
    ZoneAirTempOccHeatingSp <|-- HpbsZoneAirTempOccHeatingSp
    ZoneAirTempUnoccCoolingSp <|-- HpbsZoneAirTempUnoccCoolingSp
    ZoneAirTempUnoccHeatingSp <|-- HpbsZoneAirTempUnoccHeatingSp
    ZoneAirTempStandbyCoolingSp <|-- HpbsZoneAirTempStandbyCoolingSp
    ZoneAirTempStandbyHeatingSp <|-- HpbsZoneAirTempStandbyHeatingSp
    DischargeAirTempSensor <|-- HpbsDischargeAirTempSensor
    DischargeAirTempSp <|-- HpbsDischargeAirTempSp
    MixedAirTempSensor <|-- HpbsMixedAirTempSensor
    MixedAirTempSp <|-- HpbsMixedAirTempSp
    ReturnAirTempSensor <|-- HpbsReturnAirTempSensor
    ReturnAirTempSp <|-- HpbsReturnAirTempSp
    OutsideAirTempSensor <|-- HpbsOutsideAirTempSensor
    InletAirTempSensor <|-- HpbsInletAirTempSensor
    InletAirTempSp <|-- HpbsInletAirTempSp
    EconomizingAirTempSensor <|-- HpbsEconomizingAirTempSensor
    VentilationAirTempSensor <|-- HpbsVentilationAirTempSensor
    ZoneAirHumiditySensor <|-- HpbsZoneAirHumiditySensor
    DischargeAirHumiditySensor <|-- HpbsDischargeAirHumiditySensor
    ReturnAirHumiditySensor <|-- HpbsReturnAirHumiditySensor
    WeatherHumidityPoint <|-- HpbsOutsideAirHumiditySensor
    ZoneAirFlowSensor <|-- HpbsZoneAirFlowSensor
    ZoneAirFlowSp <|-- HpbsZoneAirFlowSp
    DischargeAirFlowSensor <|-- HpbsDischargeAirFlowSensor
    DischargeAirFlowSp <|-- HpbsDischargeAirFlowSp
    ReturnAirFlowSensor <|-- HpbsReturnAirFlowSensor
    OutsideAirFlowSensor <|-- HpbsOutsideAirFlowSensor
    OutsideAirFlowSp <|-- HpbsOutsideAirFlowSp
    ExhaustAirFlowSensor <|-- HpbsExhaustAirFlowSensor
    MixedAirFlowSensor <|-- HpbsMixedAirFlowSensor
    ZoneAirPressureSensor <|-- HpbsZoneAirPressureSensor
    ZoneAirPressureSp <|-- HpbsZoneAirPressureSp
    DischargeAirPressureSensor <|-- HpbsDischargeAirPressureSensor
    DischargeAirPressureSp <|-- HpbsDischargeAirPressureSp
    BuildingAirPressureSensor <|-- HpbsBuildingAirPressureSensor
    BuildingAirPressureSp <|-- HpbsBuildingAirPressureSp
    ZoneCo2Sensor <|-- HpbsZoneCo2Sensor
    ZoneCo2Sp <|-- HpbsZoneCo2Sp
    DischargeCo2Sensor <|-- HpbsDischargeCo2Sensor
    ReturnCo2Sensor <|-- HpbsReturnCo2Sensor
    WeatherWetbulbPoint <|-- HpbsOutsideAirWetbulbPoint
    WeatherDewPointPoint <|-- HpbsOutsideAirDewPointPoint
    FreezeStatSensor <|-- HpbsFreezeStatSensor
    FilterSensor <|-- HpbsFilterStatusSensor
    FilterPressureSensor <|-- HpbsFilterPressureDeltaSensor
    FilterPressureSensor <|-- HpbsPreFilterPressureDeltaSensor
    FilterPressureSensor <|-- HpbsFinalFilterPressureDeltaSensor
    AirHumiditySp <|-- HpbsReturnAirDehumiditySp
    BoolPoint <|-- HpbsEquipAlarmSensor
    BoolPoint <|-- HpbsFilterAlarmSensor
    BoolPoint <|-- HpbsHighTempAlarmSensor
    BoolPoint <|-- HpbsLowTempAlarmSensor
    BoolPoint <|-- HpbsSmokeAlarmSensor
    BoolPoint <|-- HpbsFireSmokeDamperAlarmSensor
    BoolPoint <|-- HpbsBoilerAlarmSensor
    BoolPoint <|-- HpbsChillerAlarmSensor
    BoilerStageCmd <|-- HpbsBoilerStageCmd
    BoilerStageSensor <|-- HpbsBoilerStageSensor
    BoilerFireRateSensor <|-- HpbsBoilerFireRateSensor
    BoilerFireRateCmd <|-- HpbsBoilerFireRateCmd
    BoilerEnableCmd <|-- HpbsBoilerEnableCmd
    BoilerRunSensor <|-- HpbsBoilerRunSensor
    BoilerLevelSensor <|-- HpbsBoilerLevelSensor
    BoilerRuntimeSensor <|-- HpbsBoilerRuntimeSensor
    ChillerStageCmd <|-- HpbsChillerStageCmd
    ChillerStageSensor <|-- HpbsChillerStageSensor
    ChillerLoadSensor <|-- HpbsChillerLoadSensor
    ChillerEnableCmd <|-- HpbsChillerEnableCmd
    ChillerRunSensor <|-- HpbsChillerRunSensor
    ChillerOilTempSensor <|-- HpbsChillerOilTempSensor
    ChillerOilHeaterCmd <|-- HpbsChillerOilHeaterCmd
    ChillerOilHeaterSensor <|-- HpbsChillerOilHeaterSensor
    ChillerRuntimeSensor <|-- HpbsChillerRuntimeSensor
    CompressorStageCmd <|-- HpbsCompressorStageCmd
    CompressorStageSensor <|-- HpbsCompressorStageSensor
    CompressorRunCmd <|-- HpbsCompressor1RunCmd
    CompressorRunSensor <|-- HpbsCompressor1RunSensor
    CompressorRunCmd <|-- HpbsCompressor2RunCmd
    CompressorRunSensor <|-- HpbsCompressor2RunSensor
    CompressorCapacitySensor <|-- HpbsCompressorCapacitySensor
    CoolingTowerStageCmd <|-- HpbsCoolingTowerStageCmd
    CoolingTowerStageSensor <|-- HpbsCoolingTowerStageSensor
    CoolingTowerEnableCmd <|-- HpbsCoolingTowerEnableCmd
    CoolingTowerRunSensor <|-- HpbsCoolingTowerRunSensor
    DamperCmd <|-- HpbsOutsideAirDamperCmd
    DamperSensor <|-- HpbsOutsideAirDamperSensor
    DamperCmd <|-- HpbsMinOutsideAirDamperCmd
    DamperSensor <|-- HpbsMinOutsideAirDamperSensor
    DamperCmd <|-- HpbsReturnAirDamperCmd
    DamperSensor <|-- HpbsReturnAirDamperSensor
    DamperCmd <|-- HpbsExhaustAirDamperCmd
    DamperSensor <|-- HpbsExhaustAirDamperSensor
    DamperCmd <|-- HpbsReliefAirDamperCmd
    DamperSensor <|-- HpbsReliefAirDamperSensor
    DamperCmd <|-- HpbsMixedAirDamperCmd
    DamperSensor <|-- HpbsMixedAirDamperSensor
    DamperCmd <|-- HpbsEconomizerDamperCmd
    DamperSensor <|-- HpbsEconomizerDamperSensor
    BoolPoint <|-- HpbsEconomizerEnableSensor
    DamperCmd <|-- HpbsZoneDamperCmd
    DamperSensor <|-- HpbsZoneDamperSensor
    DamperSp <|-- HpbsZoneMinDamperSp
    DamperSp <|-- HpbsZoneMaxDamperSp
    DamperCmd <|-- HpbsDischargeAirDamperCmd
    DamperSensor <|-- HpbsDischargeAirDamperSensor
    DamperCmd <|-- HpbsBypassDamperCmd
    DamperSensor <|-- HpbsBypassDamperSensor
    DamperSensor <|-- HpbsFireDamperSensor
    DamperSensor <|-- HpbsSmokeDamperSensor
    DamperCmd <|-- HpbsInletVaneCmd
    DamperSensor <|-- HpbsInletVaneSensor
    ThermalEnergySensor <|-- HpbsDomesticHotWaterEnergySensor
    ThermalPowerSensor <|-- HpbsDomesticHotWaterPowerSensor
    RunCmd <|-- HpbsDomesticHotWaterRecircPumpRunCmd
    RunSensor <|-- HpbsDomesticHotWaterRecircPumpRunSensor
    ElecEnergySensor <|-- HpbsBuildingElecEnergySensor
    ElecPowerSensor <|-- HpbsBuildingElecPowerSensor
    ElecPowerSensor <|-- HpbsBuildingElecDemandSensor
    ElecEnergySensor <|-- HpbsEquipElecEnergySensor
    ElecPowerSensor <|-- HpbsEquipElecPowerSensor
    ElecEnergySensor <|-- HpbsAhuElecEnergySensor
    ElecPowerSensor <|-- HpbsAhuElecPowerSensor
    ElecEnergySensor <|-- HpbsChillerElecEnergySensor
    ElecPowerSensor <|-- HpbsChillerElecPowerSensor
    NumberPoint <|-- HpbsChillerEfficiencySensor
    Ahu <|-- HpbsAhu
    Ahu <|-- HpbsAhuWithEconomizer
    Rtu <|-- HpbsRtu
    Mau <|-- HpbsMau
    Doas <|-- HpbsDoas
    Vav <|-- HpbsVav
    Vav <|-- HpbsVavReheat
    Vav <|-- HpbsVavElecReheat
    FanPoweredVav <|-- HpbsFanPoweredVav
    Boiler <|-- HpbsBoiler
    Boiler <|-- HpbsCondensingBoiler
    HotWaterBoiler <|-- HpbsHotWaterBoiler
    SteamBoiler <|-- HpbsSteamBoiler
    Chiller <|-- HpbsChiller
    AirCooledChiller <|-- HpbsAirCooledChiller
    WaterCooledChiller <|-- HpbsWaterCooledChiller
    Chiller <|-- HpbsCentrifugalChiller
    Chiller <|-- HpbsScrewChiller
    CoolingTower <|-- HpbsCoolingTower
    CoolingTower <|-- HpbsOpenCoolingTower
    CoolingTower <|-- HpbsClosedCoolingTower
    Fcu <|-- HpbsFcu
    Fcu <|-- HpbsFcu2Pipe
    Fcu <|-- HpbsFcu4Pipe
    Crac <|-- HpbsCrac
    Crah <|-- HpbsCrah
    ExhaustFan <|-- HpbsExhaustFan
    FumeHood <|-- HpbsFumeHood
    WaterHeater <|-- HpbsWaterHeater
    WaterHeater <|-- HpbsTanklessWaterHeater
    ChilledWaterPump <|-- HpbsChilledWaterPump
    HotWaterPump <|-- HpbsHotWaterPump
    CondenserWaterPump <|-- HpbsCondenserWaterPump
    HeatExchanger <|-- HpbsHeatExchanger
    HeatExchanger <|-- HpbsPlateHeatExchanger
    HeatExchanger <|-- HpbsShellTubeHeatExchanger
    HeatPump <|-- HpbsHeatPump
    AirSourceHeatPump <|-- HpbsAirSourceHeatPump
    WaterSourceHeatPump <|-- HpbsWaterSourceHeatPump
    GroundSourceHeatPump <|-- HpbsGroundSourceHeatPump
    UnitHeater <|-- HpbsUnitHeater
    RadiantEquip <|-- HpbsRadiantPanel
    RadiantEquip <|-- HpbsRadiantFloor
    ElecMeter <|-- HpbsElecMeter
    GasMeter <|-- HpbsGasMeter
    WaterMeter <|-- HpbsWaterMeter
    ThermalMeter <|-- HpbsBtuMeter
    SteamMeter <|-- HpbsSteamMeter
    FanRunCmd <|-- HpbsSupplyFanRunCmd
    FanRunSensor <|-- HpbsSupplyFanRunSensor
    FanSpeedSensor <|-- HpbsSupplyFanSpeedSensor
    FanSpeedCmd <|-- HpbsSupplyFanSpeedCmd
    VfdFreqSensor <|-- HpbsSupplyFanFreqSensor
    VfdFreqCmd <|-- HpbsSupplyFanFreqCmd
    BoolPoint <|-- HpbsSupplyFanAlarmSensor
    FanEnableCmd <|-- HpbsSupplyFanEnableCmd
    FanRunCmd <|-- HpbsReturnFanRunCmd
    FanRunSensor <|-- HpbsReturnFanRunSensor
    FanSpeedSensor <|-- HpbsReturnFanSpeedSensor
    FanSpeedCmd <|-- HpbsReturnFanSpeedCmd
    VfdFreqSensor <|-- HpbsReturnFanFreqSensor
    VfdFreqCmd <|-- HpbsReturnFanFreqCmd
    BoolPoint <|-- HpbsReturnFanAlarmSensor
    FanEnableCmd <|-- HpbsReturnFanEnableCmd
    FanRunCmd <|-- HpbsExhaustFanRunCmd
    FanRunSensor <|-- HpbsExhaustFanRunSensor
    FanSpeedSensor <|-- HpbsExhaustFanSpeedSensor
    FanSpeedCmd <|-- HpbsExhaustFanSpeedCmd
    VfdFreqSensor <|-- HpbsExhaustFanFreqSensor
    BoolPoint <|-- HpbsExhaustFanAlarmSensor
    FanRunCmd <|-- HpbsReliefFanRunCmd
    FanRunSensor <|-- HpbsReliefFanRunSensor
    FanSpeedSensor <|-- HpbsReliefFanSpeedSensor
    FanSpeedCmd <|-- HpbsReliefFanSpeedCmd
    FanRunCmd <|-- HpbsCoolingTowerFanRunCmd
    FanRunSensor <|-- HpbsCoolingTowerFanRunSensor
    FanSpeedSensor <|-- HpbsCoolingTowerFanSpeedSensor
    FanSpeedCmd <|-- HpbsCoolingTowerFanSpeedCmd
    ElecPowerSensor <|-- HpbsFanPowerSensor
    ElecEnergySensor <|-- HpbsFanEnergySensor
    ElecPowerSensor <|-- HpbsSupplyFanPowerSensor
    ElecPowerSensor <|-- HpbsReturnFanPowerSensor
    BoolPoint <|-- HpbsVfdFaultSensor
    VfdRunSensor <|-- HpbsVfdRunSensor
    VfdSpeedSensor <|-- HpbsVfdSpeedSensor
    VfdSpeedCmd <|-- HpbsVfdSpeedCmd
    EnableCmd <|-- HpbsHeatExchangerEnableCmd
    RunCmd <|-- HpbsHeatExchangerRunCmd
    RunSensor <|-- HpbsHeatExchangerRunSensor
    NumberPoint <|-- HpbsHeatExchangerRuntimeSensor
    WaterTempSensor <|-- HpbsHeatExchangerPrimaryEnteringTempSensor
    WaterTempSensor <|-- HpbsHeatExchangerPrimaryLeavingTempSensor
    WaterTempSensor <|-- HpbsHeatExchangerSecondaryEnteringTempSensor
    WaterTempSensor <|-- HpbsHeatExchangerSecondaryLeavingTempSensor
    WaterFlowSensor <|-- HpbsHeatExchangerPrimaryFlowSensor
    WaterFlowSensor <|-- HpbsHeatExchangerSecondaryFlowSensor
    ValveCmd <|-- HpbsHeatExchangerPrimaryValveCmd
    ValveSensor <|-- HpbsHeatExchangerPrimaryValveSensor
    ValveCmd <|-- HpbsHeatExchangerSecondaryValveCmd
    ValveSensor <|-- HpbsHeatExchangerSecondaryValveSensor
    NaturalGasFlowSensor <|-- HpbsNaturalGasFlowSensor
    NaturalGasFlowSensor <|-- HpbsBoilerNaturalGasFlowSensor
    NaturalGasFlowSensor <|-- HpbsDomesticWaterHeaterNaturalGasFlowSensor
    NaturalGasVolumeSensor <|-- HpbsNaturalGasVolumeSensor
    NaturalGasVolumeSensor <|-- HpbsBoilerNaturalGasVolumeSensor
    NaturalGasVolumeSensor <|-- HpbsBuildingNaturalGasVolumeSensor
    NaturalGasEnergySensor <|-- HpbsNaturalGasEnergySensor
    NaturalGasEnergySensor <|-- HpbsBoilerNaturalGasEnergySensor
    NaturalGasEnergySensor <|-- HpbsBuildingNaturalGasEnergySensor
    NaturalGasEnergySensor <|-- HpbsDomesticWaterHeaterNaturalGasEnergySensor
    NaturalGasPressureSensor <|-- HpbsNaturalGasPressureSensor
    NaturalGasPressureSensor <|-- HpbsBuildingNaturalGasPressureSensor
    ZoneOccupiedSensor <|-- HpbsZoneOccupancySensor
    ZoneOccupiedCmd <|-- HpbsZoneOccupiedCmd
    ZoneOccupiedSensor <|-- HpbsZoneOccupiedEffectiveSensor
    BoolPoint <|-- HpbsZoneOccupancyOverrideCmd
    NumberPoint <|-- HpbsZoneModeSensor
    NumberPoint <|-- HpbsZoneModeCmd
    NumberPoint <|-- HpbsAhuModeSensor
    NumberPoint <|-- HpbsAhuModeCmd
    BoolPoint <|-- HpbsEquipEnableCmd
    BoolPoint <|-- HpbsEquipRunSensor
    BoolPoint <|-- HpbsScheduleOccupiedSensor
    DateTimePoint <|-- HpbsScheduleNextOccupiedSensor
    DateTimePoint <|-- HpbsScheduleNextUnoccupiedSensor
    BoolPoint <|-- HpbsOptimalStartEnableCmd
    BoolPoint <|-- HpbsOptimalStartActiveSensor
    BoolPoint <|-- HpbsZoneOverrideActiveSensor
    NumberPoint <|-- HpbsZoneOverrideDurationSensor
    BoolPoint <|-- HpbsHeatingLockoutSensor
    NumberPoint <|-- HpbsHeatingLockoutTempSp
    BoolPoint <|-- HpbsCoolingLockoutSensor
    NumberPoint <|-- HpbsCoolingLockoutTempSp
    BoolPoint <|-- HpbsEconomizerLockoutSensor
    NumberPoint <|-- HpbsEconomizerHighLimitTempSp
    BoolPoint <|-- HpbsDcvEnableCmd
    BoolPoint <|-- HpbsDcvActiveSensor
    NumberPoint <|-- HpbsDcvMinOaFlowSp
    BoolPoint <|-- HpbsNightSetbackActiveSensor
    BoolPoint <|-- HpbsStandbyModeSensor
    BoolPoint <|-- HpbsMorningWarmupSensor
    BoolPoint <|-- HpbsMorningCooldownSensor
    Equip <|-- Fan
    Fan <|-- ExhaustFan
    Equip <|-- Pump
    Pump <|-- ChilledWaterPump
    Pump <|-- HotWaterPump
    Pump <|-- CondenserWaterPump
    Equip <|-- GasMeter
    Equip <|-- ThermalMeter
    Equip <|-- SteamMeter
    Chiller <|-- AirCooledChiller
    Chiller <|-- WaterCooledChiller
    Equip <|-- HeatPump
    HeatPump <|-- AirSourceHeatPump
    HeatPump <|-- WaterSourceHeatPump
    HeatPump <|-- GroundSourceHeatPump
    Vav <|-- FanPoweredVav
    Equip <|-- UnitHeater
    Equip <|-- Crah
    Equip <|-- WaterHeater
    NumberPoint <|-- ZoneAirFlowSensor
    NumberPoint <|-- ZoneAirFlowSp
    NumberPoint <|-- MixedAirFlowSensor
    NumberPoint <|-- ReturnAirHumiditySensor
    NumberPoint <|-- BoilerStageCmd
    NumberPoint <|-- BoilerStageSensor
    NumberPoint <|-- BoilerFireRateSensor
    NumberPoint <|-- BoilerFireRateCmd
    BoolPoint <|-- BoilerEnableCmd
    BoolPoint <|-- BoilerRunSensor
    NumberPoint <|-- BoilerLevelSensor
    NumberPoint <|-- BoilerRuntimeSensor
    NumberPoint <|-- ChillerStageCmd
    NumberPoint <|-- ChillerStageSensor
    NumberPoint <|-- ChillerLoadSensor
    BoolPoint <|-- ChillerEnableCmd
    BoolPoint <|-- ChillerRunSensor
    NumberPoint <|-- ChillerOilTempSensor
    BoolPoint <|-- ChillerOilHeaterCmd
    BoolPoint <|-- ChillerOilHeaterSensor
    NumberPoint <|-- ChillerRuntimeSensor
    NumberPoint <|-- DischargeCo2Sensor
    NumberPoint <|-- ReturnCo2Sensor
    CmdPoint <|-- CompressorCmd
    SensorPoint <|-- CompressorSensor
    CompressorCmd <|-- CompressorStageCmd
    CompressorSensor <|-- CompressorStageSensor
    CompressorCmd <|-- CompressorRunCmd
    CompressorSensor <|-- CompressorRunSensor
    CompressorSensor <|-- CompressorCapacitySensor
    NumberPoint <|-- CoolingTowerStageCmd
    NumberPoint <|-- CoolingTowerStageSensor
    BoolPoint <|-- CoolingTowerEnableCmd
    BoolPoint <|-- CoolingTowerRunSensor
    NumberPoint <|-- DamperSp
    Point <|-- FilterPoint
    FilterPoint <|-- FilterSensor
    NumberPoint <|-- FilterPressurePoint
    FilterPressurePoint <|-- FilterPressureSensor
    FilterPressurePoint <|-- FilterPressureSp
    SensorPoint <|-- HeatSensor
    SensorPoint <|-- CoolSensor
    BoolPoint <|-- FreezeStatSensor
    NumberPoint <|-- NaturalGasPressurePoint
    NaturalGasPressurePoint <|-- NaturalGasPressureSensor
    NaturalGasPressurePoint <|-- NaturalGasPressureSp
    Point <|-- DateTimePoint
    BoolPoint <|-- ZoneOccupiedCmd
    NumberPoint <|-- ZoneAirPressureSensor
    NumberPoint <|-- ZoneAirPressureSp
    NumberPoint <|-- BuildingAirPressureSensor
    NumberPoint <|-- BuildingAirPressureSp
    Point <|-- PumpPoint
    PumpPoint <|-- PumpRunSensor
    PumpPoint <|-- PumpRunCmd
    PumpPoint <|-- PumpEnableSensor
    PumpPoint <|-- PumpEnableCmd
    PumpPoint <|-- PumpSpeedSensor
    PumpPoint <|-- PumpSpeedCmd
    NumberPoint <|-- HeatStageCmd
    NumberPoint <|-- HeatStageSensor
    BoolPoint <|-- ElecHeatStageCmd
    BoolPoint <|-- ElecHeatStageSensor
    BoolPoint <|-- GasHeatStageCmd
    BoolPoint <|-- GasHeatStageSensor
    NumberPoint <|-- CoolStageCmd
    NumberPoint <|-- CoolStageSensor
    BoolPoint <|-- DxCoolStageCmd
    BoolPoint <|-- DxCoolStageSensor
    NumberPoint <|-- LeadEquipSensor
    NumberPoint <|-- EquipStagesRequestedSensor
    NumberPoint <|-- EquipStagesRunningSensor
    NumberPoint <|-- SteamFlowPoint
    SteamFlowPoint <|-- SteamFlowSensor
    SteamFlowPoint <|-- SteamFlowSp
    NumberPoint <|-- SteamPressurePoint
    SteamPressurePoint <|-- SteamPressureSensor
    SteamPressurePoint <|-- SteamPressureSp
    NumberPoint <|-- SteamTempPoint
    SteamTempPoint <|-- SteamTempSensor
    SteamTempPoint <|-- SteamTempSp
    NumberPoint <|-- SteamEnergyPoint
    SteamEnergyPoint <|-- SteamEnergySensor
    SteamEnergyPoint <|-- SteamEnergySp
    AirTempSp <|-- SystemEnableOutsideAirTempSp
    BoolPoint <|-- SystemRunSensor
    EnableCmd <|-- HotWaterSystemEnableCmd
    SystemRunSensor <|-- HotWaterSystemRunSensor
    EnableCmd <|-- ChilledWaterSystemEnableCmd
    SystemRunSensor <|-- ChilledWaterSystemRunSensor
    EnableCmd <|-- CondenserWaterSystemEnableCmd
    SystemRunSensor <|-- CondenserWaterSystemRunSensor
    EnableCmd <|-- SteamSystemEnableCmd
    SystemRunSensor <|-- SteamSystemRunSensor
    EnableCmd <|-- DomesticHotWaterSystemEnableCmd
    SystemRunSensor <|-- DomesticHotWaterSystemRunSensor
    NumberPoint <|-- ThermalEnergyPoint
    ThermalEnergyPoint <|-- ThermalEnergySensor
    ThermalEnergyPoint <|-- ThermalEnergySp
    NumberPoint <|-- ThermalPowerPoint
    ThermalPowerPoint <|-- ThermalPowerSensor
    ThermalPowerPoint <|-- ThermalPowerSp
    BoolPoint <|-- VfdRunSensor
    BoolPoint <|-- VfdRunCmd
    Dict <|-- HpbsDischargeColor
    Dict <|-- HpbsReturnColor
    Dict <|-- HpbsZoneColor
    Dict <|-- HpbsOutsideColor
    Dict <|-- HpbsMixedColor
    Dict <|-- HpbsExhaustColor
    Dict <|-- HpbsInletColor
    Dict <|-- HpbsSetpointColor
    Dict <|-- HpbsHotWaterColor
    Dict <|-- HpbsChilledWaterColor
    Dict <|-- HpbsCondenserWaterColor
    Dict <|-- HpbsDomesticHotWaterColor
    Dict <|-- HpbsSteamColor
    Dict <|-- HpbsGasColor
    Dict <|-- HpbsElecColor
    Dict <|-- HpbsSensorColor
    Dict <|-- HpbsCommandColor
    PumpRunCmd <|-- HpbsHotWaterPumpRunCmd
    PumpRunSensor <|-- HpbsHotWaterPumpRunSensor
    PumpSpeedSensor <|-- HpbsHotWaterPumpSpeedSensor
    PumpSpeedCmd <|-- HpbsHotWaterPumpSpeedCmd
    BoolPoint <|-- HpbsHotWaterPumpAlarmSensor
    PumpEnableCmd <|-- HpbsHotWaterPumpEnableCmd
    PumpRunCmd <|-- HpbsPrimaryHotWaterPumpRunCmd
    PumpRunSensor <|-- HpbsPrimaryHotWaterPumpRunSensor
    PumpRunCmd <|-- HpbsSecondaryHotWaterPumpRunCmd
    PumpRunSensor <|-- HpbsSecondaryHotWaterPumpRunSensor
    PumpSpeedSensor <|-- HpbsSecondaryHotWaterPumpSpeedSensor
    PumpRunCmd <|-- HpbsChilledWaterPumpRunCmd
    PumpRunSensor <|-- HpbsChilledWaterPumpRunSensor
    PumpSpeedSensor <|-- HpbsChilledWaterPumpSpeedSensor
    PumpSpeedCmd <|-- HpbsChilledWaterPumpSpeedCmd
    BoolPoint <|-- HpbsChilledWaterPumpAlarmSensor
    PumpEnableCmd <|-- HpbsChilledWaterPumpEnableCmd
    PumpRunCmd <|-- HpbsPrimaryChilledWaterPumpRunCmd
    PumpRunSensor <|-- HpbsPrimaryChilledWaterPumpRunSensor
    PumpRunCmd <|-- HpbsSecondaryChilledWaterPumpRunCmd
    PumpRunSensor <|-- HpbsSecondaryChilledWaterPumpRunSensor
    PumpSpeedSensor <|-- HpbsSecondaryChilledWaterPumpSpeedSensor
    PumpRunCmd <|-- HpbsCondenserWaterPumpRunCmd
    PumpRunSensor <|-- HpbsCondenserWaterPumpRunSensor
    PumpSpeedSensor <|-- HpbsCondenserWaterPumpSpeedSensor
    PumpSpeedCmd <|-- HpbsCondenserWaterPumpSpeedCmd
    BoolPoint <|-- HpbsCondenserWaterPumpAlarmSensor
    PumpRunCmd <|-- HpbsDomesticHotWaterPumpRunCmd
    PumpRunSensor <|-- HpbsDomesticHotWaterPumpRunSensor
    PumpSpeedSensor <|-- HpbsDomesticHotWaterPumpSpeedSensor
    PumpRunCmd <|-- HpbsBoosterPumpRunCmd
    PumpRunSensor <|-- HpbsBoosterPumpRunSensor
    PumpSpeedSensor <|-- HpbsBoosterPumpSpeedSensor
    ElecPowerSensor <|-- HpbsPumpPowerSensor
    ElecEnergySensor <|-- HpbsPumpEnergySensor
    ElecPowerSensor <|-- HpbsHotWaterPumpPowerSensor
    ElecPowerSensor <|-- HpbsChilledWaterPumpPowerSensor
    ElecPowerSensor <|-- HpbsCondenserWaterPumpPowerSensor
    VfdFreqSensor <|-- HpbsPumpVfdFreqSensor
    VfdFreqCmd <|-- HpbsPumpVfdFreqCmd
    BoolPoint <|-- HpbsPumpVfdFaultSensor
    HeatStageCmd <|-- HpbsHeatingStageCmd
    HeatStageSensor <|-- HpbsHeatingStageSensor
    ElecHeatStageCmd <|-- HpbsElecHeatStage1Cmd
    ElecHeatStageSensor <|-- HpbsElecHeatStage1Sensor
    ElecHeatStageCmd <|-- HpbsElecHeatStage2Cmd
    ElecHeatStageSensor <|-- HpbsElecHeatStage2Sensor
    GasHeatStageCmd <|-- HpbsGasHeatStage1Cmd
    GasHeatStageSensor <|-- HpbsGasHeatStage1Sensor
    GasHeatStageCmd <|-- HpbsGasHeatStage2Cmd
    CoolStageCmd <|-- HpbsCoolingStageCmd
    CoolStageSensor <|-- HpbsCoolingStageSensor
    DxCoolStageCmd <|-- HpbsDxCoolingStage1Cmd
    DxCoolStageSensor <|-- HpbsDxCoolingStage1Sensor
    DxCoolStageCmd <|-- HpbsDxCoolingStage2Cmd
    DxCoolStageSensor <|-- HpbsDxCoolingStage2Sensor
    LeadEquipSensor <|-- HpbsLeadEquipSensor
    EquipStagesRequestedSensor <|-- HpbsEquipStagesRequestedSensor
    EquipStagesRunningSensor <|-- HpbsEquipStagesRunningSensor
    SteamFlowSensor <|-- HpbsSteamFlowSensor
    SteamPressureSensor <|-- HpbsSteamPressureSensor
    SteamPressureSp <|-- HpbsSteamPressureSp
    SteamTempSensor <|-- HpbsSteamTempSensor
    SteamEnergySensor <|-- HpbsSteamEnergySensor
    WaterFlowSensor <|-- HpbsCondensateFlowSensor
    WaterTempSensor <|-- HpbsCondensateTempSensor
    SystemEnableOutsideAirTempSp <|-- HpbsSystemEnableOaTempSp
    HotWaterSystemEnableCmd <|-- HpbsHotWaterSystemEnableCmd
    HotWaterSystemRunSensor <|-- HpbsHotWaterSystemRunSensor
    ChilledWaterSystemEnableCmd <|-- HpbsChilledWaterSystemEnableCmd
    ChilledWaterSystemRunSensor <|-- HpbsChilledWaterSystemRunSensor
    CondenserWaterSystemEnableCmd <|-- HpbsCondenserWaterSystemEnableCmd
    CondenserWaterSystemRunSensor <|-- HpbsCondenserWaterSystemRunSensor
    SteamSystemEnableCmd <|-- HpbsSteamSystemEnableCmd
    SteamSystemRunSensor <|-- HpbsSteamSystemRunSensor
    DomesticHotWaterSystemEnableCmd <|-- HpbsDomesticHotWaterSystemEnableCmd
    DomesticHotWaterSystemRunSensor <|-- HpbsDomesticHotWaterSystemRunSensor
    ChilledWaterSystem <|-- HpbsChilledWaterSystem
    HotWaterSystem <|-- HpbsHotWaterSystem
    SteamSystem <|-- HpbsSteamSystem
    CondenserWaterSystem <|-- HpbsCondenserWaterSystem
    DomesticHotWaterSystem <|-- HpbsDomesticHotWaterSystem
    ValveCmd <|-- HpbsHotWaterValveCmd
    ValveSensor <|-- HpbsHotWaterValveSensor
    ValveCmd <|-- HpbsHeatingValveCmd
    ValveSensor <|-- HpbsHeatingValveSensor
    ValveCmd <|-- HpbsPreheatValveCmd
    ValveSensor <|-- HpbsPreheatValveSensor
    ValveCmd <|-- HpbsReheatValveCmd
    ValveSensor <|-- HpbsReheatValveSensor
    ValveCmd <|-- HpbsChilledWaterValveCmd
    ValveSensor <|-- HpbsChilledWaterValveSensor
    ValveCmd <|-- HpbsCoolingValveCmd
    ValveSensor <|-- HpbsCoolingValveSensor
    ValveCmd <|-- HpbsCondenserWaterValveCmd
    ValveSensor <|-- HpbsCondenserWaterValveSensor
    ValveCmd <|-- HpbsHotWaterBypassValveCmd
    ValveSensor <|-- HpbsHotWaterBypassValveSensor
    ValveCmd <|-- HpbsChilledWaterBypassValveCmd
    ValveSensor <|-- HpbsChilledWaterBypassValveSensor
    ValveCmd <|-- HpbsCondenserWaterBypassValveCmd
    ValveCmd <|-- HpbsHotWaterIsolationValveCmd
    ValveSensor <|-- HpbsHotWaterIsolationValveSensor
    ValveCmd <|-- HpbsChilledWaterIsolationValveCmd
    ValveSensor <|-- HpbsChilledWaterIsolationValveSensor
    ValveCmd <|-- HpbsSteamValveCmd
    ValveSensor <|-- HpbsSteamValveSensor
    ValveCmd <|-- HpbsSteamPreheatValveCmd
    ValveCmd <|-- HpbsSteamReheatValveCmd
    ValveCmd <|-- HpbsGasValveCmd
    ValveSensor <|-- HpbsGasValveSensor
    ValveCmd <|-- HpbsDomesticHotWaterRecircValveCmd
    ValveCmd <|-- HpbsDomesticHotWaterMixingValveCmd
    HotWaterEnteringTempSensor <|-- HpbsHotWaterEnteringTempSensor
    HotWaterLeavingTempSensor <|-- HpbsHotWaterLeavingTempSensor
    HotWaterLeavingTempSp <|-- HpbsHotWaterLeavingTempSp
    WaterTempSensor <|-- HpbsHotWaterSupplyTempSensor
    WaterTempSp <|-- HpbsHotWaterSupplyTempSp
    WaterTempSensor <|-- HpbsHotWaterReturnTempSensor
    WaterTempSensor <|-- HpbsHotWaterDeltaTempSensor
    ChilledWaterEnteringTempSensor <|-- HpbsChilledWaterEnteringTempSensor
    ChilledWaterLeavingTempSensor <|-- HpbsChilledWaterLeavingTempSensor
    ChilledWaterLeavingTempSp <|-- HpbsChilledWaterLeavingTempSp
    WaterTempSensor <|-- HpbsChilledWaterSupplyTempSensor
    WaterTempSp <|-- HpbsChilledWaterSupplyTempSp
    WaterTempSensor <|-- HpbsChilledWaterReturnTempSensor
    WaterTempSensor <|-- HpbsChilledWaterDeltaTempSensor
    CondenserWaterEnteringTempSensor <|-- HpbsCondenserWaterEnteringTempSensor
    CondenserWaterLeavingTempSensor <|-- HpbsCondenserWaterLeavingTempSensor
    CondenserWaterLeavingTempSp <|-- HpbsCondenserWaterLeavingTempSp
    WaterTempSensor <|-- HpbsCondenserWaterSupplyTempSensor
    WaterTempSensor <|-- HpbsCondenserWaterReturnTempSensor
    WaterTempSensor <|-- HpbsDomesticHotWaterSupplyTempSensor
    WaterTempSp <|-- HpbsDomesticHotWaterSupplyTempSp
    WaterTempSensor <|-- HpbsDomesticHotWaterReturnTempSensor
    WaterFlowSensor <|-- HpbsHotWaterFlowSensor
    WaterFlowSp <|-- HpbsHotWaterFlowSp
    WaterFlowSensor <|-- HpbsChilledWaterFlowSensor
    WaterFlowSp <|-- HpbsChilledWaterFlowSp
    WaterFlowSensor <|-- HpbsCondenserWaterFlowSensor
    WaterFlowSp <|-- HpbsCondenserWaterFlowSp
    WaterFlowSensor <|-- HpbsDomesticHotWaterFlowSensor
    WaterPressureSensor <|-- HpbsHotWaterPressureSensor
    WaterPressureSp <|-- HpbsHotWaterPressureSp
    WaterPressureSensor <|-- HpbsChilledWaterPressureSensor
    WaterPressureSp <|-- HpbsChilledWaterPressureSp
    WaterPressureSensor <|-- HpbsCondenserWaterPressureSensor
    WaterPressureSensor <|-- HpbsHotWaterDifferentialPressureSensor
    WaterPressureSp <|-- HpbsHotWaterDifferentialPressureSp
    WaterPressureSensor <|-- HpbsChilledWaterDifferentialPressureSensor
    WaterPressureSp <|-- HpbsChilledWaterDifferentialPressureSp
    WaterPressureSensor <|-- HpbsCondenserWaterDifferentialPressureSensor
    WaterVolumeSensor <|-- HpbsHotWaterVolumeSensor
    WaterVolumeSensor <|-- HpbsChilledWaterVolumeSensor
    WaterVolumeSensor <|-- HpbsCondenserWaterVolumeSensor
    WaterVolumeSensor <|-- HpbsDomesticHotWaterVolumeSensor
    ThermalEnergySensor <|-- HpbsHotWaterEnergySensor
    ThermalEnergySensor <|-- HpbsChilledWaterEnergySensor
    ThermalPowerSensor <|-- HpbsHotWaterPowerSensor
    ThermalPowerSensor <|-- HpbsChilledWaterPowerSensor
    WaterFlowSensor <|-- HpbsMakeupWaterFlowSensor
    WaterVolumeSensor <|-- HpbsMakeupWaterVolumeSensor
    WaterTempSensor <|-- HpbsCoolingTowerBasinTempSensor
    WaterTempSensor <|-- HpbsCoolingTowerApproachTempSensor

    SensorPoint <.. AirFlowSensor : mixin
    SpPoint <.. AirFlowSp : mixin
    SensorPoint <.. AirHumiditySensor : mixin
    SpPoint <.. AirHumiditySp : mixin
    SensorPoint <.. AirPressureSensor : mixin
    SpPoint <.. AirPressureSp : mixin
    SensorPoint <.. AirTempSensor : mixin
    SpPoint <.. AirTempSp : mixin
    SensorPoint <.. Co2Sensor : mixin
    SpPoint <.. Co2Sp : mixin
    SensorPoint <.. DamperSensor : mixin
    CmdPoint <.. DamperCmd : mixin
    SensorPoint <.. ElecSensor : mixin
    RunSensor <.. FanRunSensor : mixin
    RunCmd <.. FanRunCmd : mixin
    EnableSensor <.. FanEnableSensor : mixin
    EnableCmd <.. FanEnableCmd : mixin
    VfdSpeedSensor <.. FanSpeedSensor : mixin
    VfdSpeedCmd <.. FanSpeedCmd : mixin
    SpPoint <.. ZoneAirHvacModeSp : mixin
    SensorPoint <.. RunSensor : mixin
    CmdPoint <.. RunCmd : mixin
    SensorPoint <.. EnableSensor : mixin
    CmdPoint <.. EnableCmd : mixin
    SensorPoint <.. AlarmSensor : mixin
    SensorPoint <.. VfdFreqSensor : mixin
    CmdPoint <.. VfdFreqCmd : mixin
    SensorPoint <.. VfdSpeedSensor : mixin
    CmdPoint <.. VfdSpeedCmd : mixin
    SensorPoint <.. NaturalGasFlowSensor : mixin
    SpPoint <.. NaturalGasFlowSp : mixin
    SensorPoint <.. NaturalGasVolumeSensor : mixin
    SpPoint <.. NaturalGasVolumeSp : mixin
    SensorPoint <.. NaturalGasEnergySensor : mixin
    SpPoint <.. NaturalGasEnergySp : mixin
    SensorPoint <.. OccupiedSensor : mixin
    SpPoint <.. OccupiedSp : mixin
    SensorPoint <.. ValveSensor : mixin
    CmdPoint <.. ValveCmd : mixin
    SensorPoint <.. WaterFlowSensor : mixin
    SpPoint <.. WaterFlowSp : mixin
    SensorPoint <.. WaterPressureSensor : mixin
    SpPoint <.. WaterPressureSp : mixin
    SensorPoint <.. WaterTempSensor : mixin
    SpPoint <.. WaterTempSp : mixin
    SensorPoint <.. WaterVolumeSensor : mixin
    SpPoint <.. WaterVolumeSp : mixin
    EnumPoint <.. WeatherCondPoint : mixin
    BoolPoint <.. WeatherDaytimePoint : mixin
    NumberPoint <.. WeatherNumberPoint : mixin
    SpPoint <.. ElecSp : mixin
    HpbsZoneColor <.. HpbsZoneAirTempSensor : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempEffectiveSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempCoolingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempHeatingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempOccCoolingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempOccHeatingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempUnoccCoolingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempUnoccHeatingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempStandbyCoolingSp : mixin
    HpbsSetpointColor <.. HpbsZoneAirTempStandbyHeatingSp : mixin
    HpbsDischargeColor <.. HpbsDischargeAirTempSensor : mixin
    HpbsSetpointColor <.. HpbsDischargeAirTempSp : mixin
    HpbsMixedColor <.. HpbsMixedAirTempSensor : mixin
    HpbsSetpointColor <.. HpbsMixedAirTempSp : mixin
    HpbsReturnColor <.. HpbsReturnAirTempSensor : mixin
    HpbsSetpointColor <.. HpbsReturnAirTempSp : mixin
    HpbsOutsideColor <.. HpbsOutsideAirTempSensor : mixin
    HpbsInletColor <.. HpbsInletAirTempSensor : mixin
    HpbsSetpointColor <.. HpbsInletAirTempSp : mixin
    HpbsOutsideColor <.. HpbsEconomizingAirTempSensor : mixin
    HpbsOutsideColor <.. HpbsVentilationAirTempSensor : mixin
    HpbsZoneColor <.. HpbsZoneAirHumiditySensor : mixin
    HpbsDischargeColor <.. HpbsDischargeAirHumiditySensor : mixin
    HpbsReturnColor <.. HpbsReturnAirHumiditySensor : mixin
    HpbsOutsideColor <.. HpbsOutsideAirHumiditySensor : mixin
    HpbsZoneColor <.. HpbsZoneAirFlowSensor : mixin
    HpbsSetpointColor <.. HpbsZoneAirFlowSp : mixin
    HpbsDischargeColor <.. HpbsDischargeAirFlowSensor : mixin
    HpbsSetpointColor <.. HpbsDischargeAirFlowSp : mixin
    HpbsReturnColor <.. HpbsReturnAirFlowSensor : mixin
    HpbsOutsideColor <.. HpbsOutsideAirFlowSensor : mixin
    HpbsSetpointColor <.. HpbsOutsideAirFlowSp : mixin
    HpbsExhaustColor <.. HpbsExhaustAirFlowSensor : mixin
    HpbsMixedColor <.. HpbsMixedAirFlowSensor : mixin
    HpbsZoneColor <.. HpbsZoneAirPressureSensor : mixin
    HpbsSetpointColor <.. HpbsZoneAirPressureSp : mixin
    HpbsDischargeColor <.. HpbsDischargeAirPressureSensor : mixin
    HpbsSetpointColor <.. HpbsDischargeAirPressureSp : mixin
    HpbsZoneColor <.. HpbsBuildingAirPressureSensor : mixin
    HpbsSetpointColor <.. HpbsBuildingAirPressureSp : mixin
    HpbsZoneColor <.. HpbsZoneCo2Sensor : mixin
    HpbsSetpointColor <.. HpbsZoneCo2Sp : mixin
    HpbsDischargeColor <.. HpbsDischargeCo2Sensor : mixin
    HpbsReturnColor <.. HpbsReturnCo2Sensor : mixin
    HpbsOutsideColor <.. HpbsOutsideAirWetbulbPoint : mixin
    HpbsOutsideColor <.. HpbsOutsideAirDewPointPoint : mixin
    HpbsSensorColor <.. HpbsFreezeStatSensor : mixin
    HpbsSensorColor <.. HpbsFilterStatusSensor : mixin
    HpbsSensorColor <.. HpbsFilterPressureDeltaSensor : mixin
    HpbsSensorColor <.. HpbsPreFilterPressureDeltaSensor : mixin
    HpbsSensorColor <.. HpbsFinalFilterPressureDeltaSensor : mixin
    HpbsSetpointColor <.. HpbsReturnAirDehumiditySp : mixin
    SensorPoint <.. HpbsEquipAlarmSensor : mixin
    HpbsSensorColor <.. HpbsEquipAlarmSensor : mixin
    SensorPoint <.. HpbsFilterAlarmSensor : mixin
    HpbsSensorColor <.. HpbsFilterAlarmSensor : mixin
    SensorPoint <.. HpbsHighTempAlarmSensor : mixin
    HpbsSensorColor <.. HpbsHighTempAlarmSensor : mixin
    SensorPoint <.. HpbsLowTempAlarmSensor : mixin
    HpbsSensorColor <.. HpbsLowTempAlarmSensor : mixin
    SensorPoint <.. HpbsSmokeAlarmSensor : mixin
    HpbsSensorColor <.. HpbsSmokeAlarmSensor : mixin
    SensorPoint <.. HpbsFireSmokeDamperAlarmSensor : mixin
    HpbsSensorColor <.. HpbsFireSmokeDamperAlarmSensor : mixin
    SensorPoint <.. HpbsBoilerAlarmSensor : mixin
    HpbsHotWaterColor <.. HpbsBoilerAlarmSensor : mixin
    SensorPoint <.. HpbsChillerAlarmSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerAlarmSensor : mixin
    HpbsHotWaterColor <.. HpbsBoilerStageCmd : mixin
    HpbsHotWaterColor <.. HpbsBoilerStageSensor : mixin
    HpbsHotWaterColor <.. HpbsBoilerFireRateSensor : mixin
    HpbsSetpointColor <.. HpbsBoilerFireRateCmd : mixin
    HpbsHotWaterColor <.. HpbsBoilerEnableCmd : mixin
    HpbsHotWaterColor <.. HpbsBoilerRunSensor : mixin
    HpbsHotWaterColor <.. HpbsBoilerLevelSensor : mixin
    HpbsHotWaterColor <.. HpbsBoilerRuntimeSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerStageCmd : mixin
    HpbsChilledWaterColor <.. HpbsChillerStageSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerLoadSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerEnableCmd : mixin
    HpbsChilledWaterColor <.. HpbsChillerRunSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerOilTempSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerOilHeaterCmd : mixin
    HpbsChilledWaterColor <.. HpbsChillerOilHeaterSensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerRuntimeSensor : mixin
    HpbsChilledWaterColor <.. HpbsCompressorStageCmd : mixin
    HpbsChilledWaterColor <.. HpbsCompressorStageSensor : mixin
    HpbsChilledWaterColor <.. HpbsCompressor1RunCmd : mixin
    HpbsChilledWaterColor <.. HpbsCompressor1RunSensor : mixin
    HpbsChilledWaterColor <.. HpbsCompressor2RunCmd : mixin
    HpbsChilledWaterColor <.. HpbsCompressor2RunSensor : mixin
    HpbsChilledWaterColor <.. HpbsCompressorCapacitySensor : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerStageCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerStageSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerEnableCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerRunSensor : mixin
    HpbsOutsideColor <.. HpbsOutsideAirDamperCmd : mixin
    HpbsOutsideColor <.. HpbsOutsideAirDamperSensor : mixin
    HpbsOutsideColor <.. HpbsMinOutsideAirDamperCmd : mixin
    HpbsOutsideColor <.. HpbsMinOutsideAirDamperSensor : mixin
    HpbsReturnColor <.. HpbsReturnAirDamperCmd : mixin
    HpbsReturnColor <.. HpbsReturnAirDamperSensor : mixin
    HpbsExhaustColor <.. HpbsExhaustAirDamperCmd : mixin
    HpbsExhaustColor <.. HpbsExhaustAirDamperSensor : mixin
    HpbsExhaustColor <.. HpbsReliefAirDamperCmd : mixin
    HpbsExhaustColor <.. HpbsReliefAirDamperSensor : mixin
    HpbsMixedColor <.. HpbsMixedAirDamperCmd : mixin
    HpbsMixedColor <.. HpbsMixedAirDamperSensor : mixin
    HpbsOutsideColor <.. HpbsEconomizerDamperCmd : mixin
    HpbsOutsideColor <.. HpbsEconomizerDamperSensor : mixin
    SensorPoint <.. HpbsEconomizerEnableSensor : mixin
    HpbsOutsideColor <.. HpbsEconomizerEnableSensor : mixin
    HpbsZoneColor <.. HpbsZoneDamperCmd : mixin
    HpbsZoneColor <.. HpbsZoneDamperSensor : mixin
    HpbsSetpointColor <.. HpbsZoneMinDamperSp : mixin
    HpbsSetpointColor <.. HpbsZoneMaxDamperSp : mixin
    HpbsDischargeColor <.. HpbsDischargeAirDamperCmd : mixin
    HpbsDischargeColor <.. HpbsDischargeAirDamperSensor : mixin
    HpbsSensorColor <.. HpbsBypassDamperCmd : mixin
    HpbsSensorColor <.. HpbsBypassDamperSensor : mixin
    HpbsSensorColor <.. HpbsFireDamperSensor : mixin
    HpbsSensorColor <.. HpbsSmokeDamperSensor : mixin
    HpbsInletColor <.. HpbsInletVaneCmd : mixin
    HpbsInletColor <.. HpbsInletVaneSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterEnergySensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterPowerSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterRecircPumpRunCmd : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterRecircPumpRunSensor : mixin
    HpbsElecColor <.. HpbsBuildingElecEnergySensor : mixin
    HpbsElecColor <.. HpbsBuildingElecPowerSensor : mixin
    HpbsElecColor <.. HpbsBuildingElecDemandSensor : mixin
    HpbsElecColor <.. HpbsEquipElecEnergySensor : mixin
    HpbsElecColor <.. HpbsEquipElecPowerSensor : mixin
    HpbsElecColor <.. HpbsAhuElecEnergySensor : mixin
    HpbsElecColor <.. HpbsAhuElecPowerSensor : mixin
    HpbsElecColor <.. HpbsChillerElecEnergySensor : mixin
    HpbsElecColor <.. HpbsChillerElecPowerSensor : mixin
    SensorPoint <.. HpbsChillerEfficiencySensor : mixin
    HpbsChilledWaterColor <.. HpbsChillerEfficiencySensor : mixin
    HpbsDischargeColor <.. HpbsSupplyFanRunCmd : mixin
    HpbsDischargeColor <.. HpbsSupplyFanRunSensor : mixin
    HpbsDischargeColor <.. HpbsSupplyFanSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsSupplyFanSpeedCmd : mixin
    HpbsDischargeColor <.. HpbsSupplyFanFreqSensor : mixin
    HpbsSetpointColor <.. HpbsSupplyFanFreqCmd : mixin
    SensorPoint <.. HpbsSupplyFanAlarmSensor : mixin
    HpbsDischargeColor <.. HpbsSupplyFanAlarmSensor : mixin
    HpbsDischargeColor <.. HpbsSupplyFanEnableCmd : mixin
    HpbsReturnColor <.. HpbsReturnFanRunCmd : mixin
    HpbsReturnColor <.. HpbsReturnFanRunSensor : mixin
    HpbsReturnColor <.. HpbsReturnFanSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsReturnFanSpeedCmd : mixin
    HpbsReturnColor <.. HpbsReturnFanFreqSensor : mixin
    HpbsSetpointColor <.. HpbsReturnFanFreqCmd : mixin
    SensorPoint <.. HpbsReturnFanAlarmSensor : mixin
    HpbsReturnColor <.. HpbsReturnFanAlarmSensor : mixin
    HpbsReturnColor <.. HpbsReturnFanEnableCmd : mixin
    HpbsExhaustColor <.. HpbsExhaustFanRunCmd : mixin
    HpbsExhaustColor <.. HpbsExhaustFanRunSensor : mixin
    HpbsExhaustColor <.. HpbsExhaustFanSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsExhaustFanSpeedCmd : mixin
    HpbsExhaustColor <.. HpbsExhaustFanFreqSensor : mixin
    SensorPoint <.. HpbsExhaustFanAlarmSensor : mixin
    HpbsExhaustColor <.. HpbsExhaustFanAlarmSensor : mixin
    HpbsExhaustColor <.. HpbsReliefFanRunCmd : mixin
    HpbsExhaustColor <.. HpbsReliefFanRunSensor : mixin
    HpbsExhaustColor <.. HpbsReliefFanSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsReliefFanSpeedCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerFanRunCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerFanRunSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerFanSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsCoolingTowerFanSpeedCmd : mixin
    HpbsElecColor <.. HpbsFanPowerSensor : mixin
    HpbsElecColor <.. HpbsFanEnergySensor : mixin
    HpbsElecColor <.. HpbsSupplyFanPowerSensor : mixin
    HpbsElecColor <.. HpbsReturnFanPowerSensor : mixin
    SensorPoint <.. HpbsVfdFaultSensor : mixin
    HpbsSensorColor <.. HpbsVfdFaultSensor : mixin
    HpbsSensorColor <.. HpbsVfdRunSensor : mixin
    HpbsSensorColor <.. HpbsVfdSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsVfdSpeedCmd : mixin
    HpbsCommandColor <.. HpbsHeatExchangerEnableCmd : mixin
    HpbsCommandColor <.. HpbsHeatExchangerRunCmd : mixin
    HpbsSensorColor <.. HpbsHeatExchangerRunSensor : mixin
    SensorPoint <.. HpbsHeatExchangerRuntimeSensor : mixin
    HpbsSensorColor <.. HpbsHeatExchangerRuntimeSensor : mixin
    HpbsHotWaterColor <.. HpbsHeatExchangerPrimaryEnteringTempSensor : mixin
    HpbsHotWaterColor <.. HpbsHeatExchangerPrimaryLeavingTempSensor : mixin
    HpbsChilledWaterColor <.. HpbsHeatExchangerSecondaryEnteringTempSensor : mixin
    HpbsChilledWaterColor <.. HpbsHeatExchangerSecondaryLeavingTempSensor : mixin
    HpbsHotWaterColor <.. HpbsHeatExchangerPrimaryFlowSensor : mixin
    HpbsChilledWaterColor <.. HpbsHeatExchangerSecondaryFlowSensor : mixin
    HpbsSetpointColor <.. HpbsHeatExchangerPrimaryValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHeatExchangerPrimaryValveSensor : mixin
    HpbsSetpointColor <.. HpbsHeatExchangerSecondaryValveCmd : mixin
    HpbsChilledWaterColor <.. HpbsHeatExchangerSecondaryValveSensor : mixin
    HpbsGasColor <.. HpbsNaturalGasFlowSensor : mixin
    HpbsGasColor <.. HpbsBoilerNaturalGasFlowSensor : mixin
    HpbsGasColor <.. HpbsDomesticWaterHeaterNaturalGasFlowSensor : mixin
    HpbsGasColor <.. HpbsNaturalGasVolumeSensor : mixin
    HpbsGasColor <.. HpbsBoilerNaturalGasVolumeSensor : mixin
    HpbsGasColor <.. HpbsBuildingNaturalGasVolumeSensor : mixin
    HpbsGasColor <.. HpbsNaturalGasEnergySensor : mixin
    HpbsGasColor <.. HpbsBoilerNaturalGasEnergySensor : mixin
    HpbsGasColor <.. HpbsBuildingNaturalGasEnergySensor : mixin
    HpbsGasColor <.. HpbsDomesticWaterHeaterNaturalGasEnergySensor : mixin
    HpbsGasColor <.. HpbsNaturalGasPressureSensor : mixin
    HpbsGasColor <.. HpbsBuildingNaturalGasPressureSensor : mixin
    HpbsZoneColor <.. HpbsZoneOccupancySensor : mixin
    HpbsZoneColor <.. HpbsZoneOccupiedCmd : mixin
    HpbsZoneColor <.. HpbsZoneOccupiedEffectiveSensor : mixin
    CmdPoint <.. HpbsZoneOccupancyOverrideCmd : mixin
    HpbsZoneColor <.. HpbsZoneOccupancyOverrideCmd : mixin
    SensorPoint <.. HpbsZoneModeSensor : mixin
    HpbsZoneColor <.. HpbsZoneModeSensor : mixin
    CmdPoint <.. HpbsZoneModeCmd : mixin
    HpbsZoneColor <.. HpbsZoneModeCmd : mixin
    SensorPoint <.. HpbsAhuModeSensor : mixin
    HpbsSensorColor <.. HpbsAhuModeSensor : mixin
    CmdPoint <.. HpbsAhuModeCmd : mixin
    HpbsSensorColor <.. HpbsAhuModeCmd : mixin
    CmdPoint <.. HpbsEquipEnableCmd : mixin
    HpbsSensorColor <.. HpbsEquipEnableCmd : mixin
    SensorPoint <.. HpbsEquipRunSensor : mixin
    HpbsSensorColor <.. HpbsEquipRunSensor : mixin
    SensorPoint <.. HpbsScheduleOccupiedSensor : mixin
    HpbsSensorColor <.. HpbsScheduleOccupiedSensor : mixin
    SensorPoint <.. HpbsScheduleNextOccupiedSensor : mixin
    HpbsSensorColor <.. HpbsScheduleNextOccupiedSensor : mixin
    SensorPoint <.. HpbsScheduleNextUnoccupiedSensor : mixin
    HpbsSensorColor <.. HpbsScheduleNextUnoccupiedSensor : mixin
    CmdPoint <.. HpbsOptimalStartEnableCmd : mixin
    HpbsSensorColor <.. HpbsOptimalStartEnableCmd : mixin
    SensorPoint <.. HpbsOptimalStartActiveSensor : mixin
    HpbsSensorColor <.. HpbsOptimalStartActiveSensor : mixin
    SensorPoint <.. HpbsZoneOverrideActiveSensor : mixin
    HpbsZoneColor <.. HpbsZoneOverrideActiveSensor : mixin
    SensorPoint <.. HpbsZoneOverrideDurationSensor : mixin
    HpbsZoneColor <.. HpbsZoneOverrideDurationSensor : mixin
    SensorPoint <.. HpbsHeatingLockoutSensor : mixin
    HpbsHotWaterColor <.. HpbsHeatingLockoutSensor : mixin
    SpPoint <.. HpbsHeatingLockoutTempSp : mixin
    HpbsSetpointColor <.. HpbsHeatingLockoutTempSp : mixin
    SensorPoint <.. HpbsCoolingLockoutSensor : mixin
    HpbsChilledWaterColor <.. HpbsCoolingLockoutSensor : mixin
    SpPoint <.. HpbsCoolingLockoutTempSp : mixin
    HpbsSetpointColor <.. HpbsCoolingLockoutTempSp : mixin
    SensorPoint <.. HpbsEconomizerLockoutSensor : mixin
    HpbsOutsideColor <.. HpbsEconomizerLockoutSensor : mixin
    SpPoint <.. HpbsEconomizerHighLimitTempSp : mixin
    HpbsSetpointColor <.. HpbsEconomizerHighLimitTempSp : mixin
    CmdPoint <.. HpbsDcvEnableCmd : mixin
    HpbsOutsideColor <.. HpbsDcvEnableCmd : mixin
    SensorPoint <.. HpbsDcvActiveSensor : mixin
    HpbsOutsideColor <.. HpbsDcvActiveSensor : mixin
    SpPoint <.. HpbsDcvMinOaFlowSp : mixin
    HpbsSetpointColor <.. HpbsDcvMinOaFlowSp : mixin
    SensorPoint <.. HpbsNightSetbackActiveSensor : mixin
    HpbsSensorColor <.. HpbsNightSetbackActiveSensor : mixin
    SensorPoint <.. HpbsStandbyModeSensor : mixin
    HpbsSensorColor <.. HpbsStandbyModeSensor : mixin
    SensorPoint <.. HpbsMorningWarmupSensor : mixin
    HpbsHotWaterColor <.. HpbsMorningWarmupSensor : mixin
    SensorPoint <.. HpbsMorningCooldownSensor : mixin
    HpbsChilledWaterColor <.. HpbsMorningCooldownSensor : mixin
    SensorPoint <.. ZoneAirFlowSensor : mixin
    SpPoint <.. ZoneAirFlowSp : mixin
    SensorPoint <.. MixedAirFlowSensor : mixin
    SensorPoint <.. ReturnAirHumiditySensor : mixin
    CmdPoint <.. BoilerStageCmd : mixin
    SensorPoint <.. BoilerStageSensor : mixin
    SensorPoint <.. BoilerFireRateSensor : mixin
    CmdPoint <.. BoilerFireRateCmd : mixin
    CmdPoint <.. BoilerEnableCmd : mixin
    SensorPoint <.. BoilerRunSensor : mixin
    SensorPoint <.. BoilerLevelSensor : mixin
    SensorPoint <.. BoilerRuntimeSensor : mixin
    CmdPoint <.. ChillerStageCmd : mixin
    SensorPoint <.. ChillerStageSensor : mixin
    SensorPoint <.. ChillerLoadSensor : mixin
    CmdPoint <.. ChillerEnableCmd : mixin
    SensorPoint <.. ChillerRunSensor : mixin
    SensorPoint <.. ChillerOilTempSensor : mixin
    CmdPoint <.. ChillerOilHeaterCmd : mixin
    SensorPoint <.. ChillerOilHeaterSensor : mixin
    SensorPoint <.. ChillerRuntimeSensor : mixin
    SensorPoint <.. DischargeCo2Sensor : mixin
    SensorPoint <.. ReturnCo2Sensor : mixin
    NumberPoint <.. CompressorStageCmd : mixin
    NumberPoint <.. CompressorStageSensor : mixin
    BoolPoint <.. CompressorRunCmd : mixin
    BoolPoint <.. CompressorRunSensor : mixin
    NumberPoint <.. CompressorCapacitySensor : mixin
    CmdPoint <.. CoolingTowerStageCmd : mixin
    SensorPoint <.. CoolingTowerStageSensor : mixin
    CmdPoint <.. CoolingTowerEnableCmd : mixin
    SensorPoint <.. CoolingTowerRunSensor : mixin
    SpPoint <.. DamperSp : mixin
    AlarmSensor <.. FilterSensor : mixin
    SensorPoint <.. FilterPressureSensor : mixin
    SpPoint <.. FilterPressureSp : mixin
    SensorPoint <.. FreezeStatSensor : mixin
    SensorPoint <.. NaturalGasPressureSensor : mixin
    SpPoint <.. NaturalGasPressureSp : mixin
    CmdPoint <.. ZoneOccupiedCmd : mixin
    SensorPoint <.. ZoneAirPressureSensor : mixin
    SpPoint <.. ZoneAirPressureSp : mixin
    SensorPoint <.. BuildingAirPressureSensor : mixin
    SpPoint <.. BuildingAirPressureSp : mixin
    RunSensor <.. PumpRunSensor : mixin
    RunCmd <.. PumpRunCmd : mixin
    EnableSensor <.. PumpEnableSensor : mixin
    EnableCmd <.. PumpEnableCmd : mixin
    VfdSpeedSensor <.. PumpSpeedSensor : mixin
    VfdSpeedCmd <.. PumpSpeedCmd : mixin
    CmdPoint <.. HeatStageCmd : mixin
    SensorPoint <.. HeatStageSensor : mixin
    CmdPoint <.. ElecHeatStageCmd : mixin
    SensorPoint <.. ElecHeatStageSensor : mixin
    CmdPoint <.. GasHeatStageCmd : mixin
    SensorPoint <.. GasHeatStageSensor : mixin
    CmdPoint <.. CoolStageCmd : mixin
    SensorPoint <.. CoolStageSensor : mixin
    CmdPoint <.. DxCoolStageCmd : mixin
    SensorPoint <.. DxCoolStageSensor : mixin
    SensorPoint <.. LeadEquipSensor : mixin
    SensorPoint <.. EquipStagesRequestedSensor : mixin
    SensorPoint <.. EquipStagesRunningSensor : mixin
    SensorPoint <.. SteamFlowSensor : mixin
    SpPoint <.. SteamFlowSp : mixin
    SensorPoint <.. SteamPressureSensor : mixin
    SpPoint <.. SteamPressureSp : mixin
    SensorPoint <.. SteamTempSensor : mixin
    SpPoint <.. SteamTempSp : mixin
    SensorPoint <.. SteamEnergySensor : mixin
    SpPoint <.. SteamEnergySp : mixin
    SensorPoint <.. SystemRunSensor : mixin
    SensorPoint <.. ThermalEnergySensor : mixin
    SpPoint <.. ThermalEnergySp : mixin
    SensorPoint <.. ThermalPowerSensor : mixin
    SpPoint <.. ThermalPowerSp : mixin
    SensorPoint <.. VfdRunSensor : mixin
    CmdPoint <.. VfdRunCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPumpRunCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPumpRunSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPumpSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsHotWaterPumpSpeedCmd : mixin
    SensorPoint <.. HpbsHotWaterPumpAlarmSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPumpAlarmSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPumpEnableCmd : mixin
    HpbsHotWaterColor <.. HpbsPrimaryHotWaterPumpRunCmd : mixin
    HpbsHotWaterColor <.. HpbsPrimaryHotWaterPumpRunSensor : mixin
    HpbsHotWaterColor <.. HpbsSecondaryHotWaterPumpRunCmd : mixin
    HpbsHotWaterColor <.. HpbsSecondaryHotWaterPumpRunSensor : mixin
    HpbsHotWaterColor <.. HpbsSecondaryHotWaterPumpSpeedSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPumpRunCmd : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPumpRunSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPumpSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsChilledWaterPumpSpeedCmd : mixin
    SensorPoint <.. HpbsChilledWaterPumpAlarmSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPumpAlarmSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPumpEnableCmd : mixin
    HpbsChilledWaterColor <.. HpbsPrimaryChilledWaterPumpRunCmd : mixin
    HpbsChilledWaterColor <.. HpbsPrimaryChilledWaterPumpRunSensor : mixin
    HpbsChilledWaterColor <.. HpbsSecondaryChilledWaterPumpRunCmd : mixin
    HpbsChilledWaterColor <.. HpbsSecondaryChilledWaterPumpRunSensor : mixin
    HpbsChilledWaterColor <.. HpbsSecondaryChilledWaterPumpSpeedSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterPumpRunCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterPumpRunSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterPumpSpeedSensor : mixin
    HpbsSetpointColor <.. HpbsCondenserWaterPumpSpeedCmd : mixin
    SensorPoint <.. HpbsCondenserWaterPumpAlarmSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterPumpAlarmSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterPumpRunCmd : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterPumpRunSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterPumpSpeedSensor : mixin
    HpbsSensorColor <.. HpbsBoosterPumpRunCmd : mixin
    HpbsSensorColor <.. HpbsBoosterPumpRunSensor : mixin
    HpbsSensorColor <.. HpbsBoosterPumpSpeedSensor : mixin
    HpbsElecColor <.. HpbsPumpPowerSensor : mixin
    HpbsElecColor <.. HpbsPumpEnergySensor : mixin
    HpbsElecColor <.. HpbsHotWaterPumpPowerSensor : mixin
    HpbsElecColor <.. HpbsChilledWaterPumpPowerSensor : mixin
    HpbsElecColor <.. HpbsCondenserWaterPumpPowerSensor : mixin
    HpbsSensorColor <.. HpbsPumpVfdFreqSensor : mixin
    HpbsSetpointColor <.. HpbsPumpVfdFreqCmd : mixin
    SensorPoint <.. HpbsPumpVfdFaultSensor : mixin
    HpbsSensorColor <.. HpbsPumpVfdFaultSensor : mixin
    HpbsHotWaterColor <.. HpbsHeatingStageCmd : mixin
    HpbsHotWaterColor <.. HpbsHeatingStageSensor : mixin
    HpbsElecColor <.. HpbsElecHeatStage1Cmd : mixin
    HpbsElecColor <.. HpbsElecHeatStage1Sensor : mixin
    HpbsElecColor <.. HpbsElecHeatStage2Cmd : mixin
    HpbsElecColor <.. HpbsElecHeatStage2Sensor : mixin
    HpbsGasColor <.. HpbsGasHeatStage1Cmd : mixin
    HpbsGasColor <.. HpbsGasHeatStage1Sensor : mixin
    HpbsGasColor <.. HpbsGasHeatStage2Cmd : mixin
    HpbsChilledWaterColor <.. HpbsCoolingStageCmd : mixin
    HpbsChilledWaterColor <.. HpbsCoolingStageSensor : mixin
    HpbsChilledWaterColor <.. HpbsDxCoolingStage1Cmd : mixin
    HpbsChilledWaterColor <.. HpbsDxCoolingStage1Sensor : mixin
    HpbsChilledWaterColor <.. HpbsDxCoolingStage2Cmd : mixin
    HpbsChilledWaterColor <.. HpbsDxCoolingStage2Sensor : mixin
    HpbsSensorColor <.. HpbsLeadEquipSensor : mixin
    HpbsSensorColor <.. HpbsEquipStagesRequestedSensor : mixin
    HpbsSensorColor <.. HpbsEquipStagesRunningSensor : mixin
    HpbsSteamColor <.. HpbsSteamFlowSensor : mixin
    HpbsSteamColor <.. HpbsSteamPressureSensor : mixin
    HpbsSetpointColor <.. HpbsSteamPressureSp : mixin
    HpbsSteamColor <.. HpbsSteamTempSensor : mixin
    HpbsSteamColor <.. HpbsSteamEnergySensor : mixin
    HpbsSteamColor <.. HpbsCondensateFlowSensor : mixin
    HpbsSteamColor <.. HpbsCondensateTempSensor : mixin
    HpbsSetpointColor <.. HpbsSystemEnableOaTempSp : mixin
    HpbsHotWaterColor <.. HpbsHotWaterSystemEnableCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterSystemRunSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterSystemEnableCmd : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterSystemRunSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterSystemEnableCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterSystemRunSensor : mixin
    HpbsSteamColor <.. HpbsSteamSystemEnableCmd : mixin
    HpbsSteamColor <.. HpbsSteamSystemRunSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterSystemEnableCmd : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterSystemRunSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterValveSensor : mixin
    HpbsHotWaterColor <.. HpbsHeatingValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHeatingValveSensor : mixin
    HpbsHotWaterColor <.. HpbsPreheatValveCmd : mixin
    HpbsHotWaterColor <.. HpbsPreheatValveSensor : mixin
    HpbsHotWaterColor <.. HpbsReheatValveCmd : mixin
    HpbsHotWaterColor <.. HpbsReheatValveSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterValveCmd : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterValveSensor : mixin
    HpbsChilledWaterColor <.. HpbsCoolingValveCmd : mixin
    HpbsChilledWaterColor <.. HpbsCoolingValveSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterValveCmd : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterValveSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterBypassValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterBypassValveSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterBypassValveCmd : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterBypassValveSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterBypassValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterIsolationValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterIsolationValveSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterIsolationValveCmd : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterIsolationValveSensor : mixin
    HpbsSteamColor <.. HpbsSteamValveCmd : mixin
    HpbsSteamColor <.. HpbsSteamValveSensor : mixin
    HpbsSteamColor <.. HpbsSteamPreheatValveCmd : mixin
    HpbsSteamColor <.. HpbsSteamReheatValveCmd : mixin
    HpbsGasColor <.. HpbsGasValveCmd : mixin
    HpbsGasColor <.. HpbsGasValveSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterRecircValveCmd : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterMixingValveCmd : mixin
    HpbsHotWaterColor <.. HpbsHotWaterEnteringTempSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterLeavingTempSensor : mixin
    HpbsSetpointColor <.. HpbsHotWaterLeavingTempSp : mixin
    HpbsHotWaterColor <.. HpbsHotWaterSupplyTempSensor : mixin
    HpbsSetpointColor <.. HpbsHotWaterSupplyTempSp : mixin
    HpbsHotWaterColor <.. HpbsHotWaterReturnTempSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterDeltaTempSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterEnteringTempSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterLeavingTempSensor : mixin
    HpbsSetpointColor <.. HpbsChilledWaterLeavingTempSp : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterSupplyTempSensor : mixin
    HpbsSetpointColor <.. HpbsChilledWaterSupplyTempSp : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterReturnTempSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterDeltaTempSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterEnteringTempSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterLeavingTempSensor : mixin
    HpbsSetpointColor <.. HpbsCondenserWaterLeavingTempSp : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterSupplyTempSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterReturnTempSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterSupplyTempSensor : mixin
    HpbsSetpointColor <.. HpbsDomesticHotWaterSupplyTempSp : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterReturnTempSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterFlowSensor : mixin
    HpbsSetpointColor <.. HpbsHotWaterFlowSp : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterFlowSensor : mixin
    HpbsSetpointColor <.. HpbsChilledWaterFlowSp : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterFlowSensor : mixin
    HpbsSetpointColor <.. HpbsCondenserWaterFlowSp : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterFlowSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPressureSensor : mixin
    HpbsSetpointColor <.. HpbsHotWaterPressureSp : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPressureSensor : mixin
    HpbsSetpointColor <.. HpbsChilledWaterPressureSp : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterPressureSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterDifferentialPressureSensor : mixin
    HpbsSetpointColor <.. HpbsHotWaterDifferentialPressureSp : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterDifferentialPressureSensor : mixin
    HpbsSetpointColor <.. HpbsChilledWaterDifferentialPressureSp : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterDifferentialPressureSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterVolumeSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterVolumeSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCondenserWaterVolumeSensor : mixin
    HpbsDomesticHotWaterColor <.. HpbsDomesticHotWaterVolumeSensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterEnergySensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterEnergySensor : mixin
    HpbsHotWaterColor <.. HpbsHotWaterPowerSensor : mixin
    HpbsChilledWaterColor <.. HpbsChilledWaterPowerSensor : mixin
    HpbsSensorColor <.. HpbsMakeupWaterFlowSensor : mixin
    HpbsSensorColor <.. HpbsMakeupWaterVolumeSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerBasinTempSensor : mixin
    HpbsCondenserWaterColor <.. HpbsCoolingTowerApproachTempSensor : mixin

    class Scalar {
        <<abstract>>
    }
    class Seq {
        <<abstract>>
    }
    class Entity {
        <<abstract>>
    }
    class Attr {
        <<abstract>>
    }
    class PhEntity {
        <<abstract>>
    }
    class Equip {
        <<abstract>>
    }
    class AirHandlingEquip {
        <<abstract>>
    }
    class AirTerminalUnit {
        <<abstract>>
    }
    class Coil {
        <<abstract>>
    }
    class Conduit {
        <<abstract>>
    }
    class RadiantEquip {
        <<abstract>>
    }
    class VerticalTransport {
        <<abstract>>
    }
    class Feature {
        <<abstract>>
    }
    class Point {
        <<abstract>>
    }
    class CurPoint {
        <<abstract>>
    }
    class HisPoint {
        <<abstract>>
    }
    class WritablePoint {
        <<abstract>>
    }
    class SyntheticPoint {
        <<abstract>>
    }
    class ComputedPoint {
        <<abstract>>
    }
    class MlPoint {
        <<abstract>>
    }
    class SimPoint {
        <<abstract>>
    }
    class GeoPlace {
        <<abstract>>
    }
    class Space {
        <<abstract>>
    }
    class WeatherPoint {
        <<abstract>>
    }
    class AirFlowPoint {
        <<abstract>>
    }
    class AirFlowSensor {
        <<abstract>>
    }
    class AirFlowSp {
        <<abstract>>
    }
    class AirHumidityPoint {
        <<abstract>>
    }
    class AirHumiditySensor {
        <<abstract>>
    }
    class AirHumiditySp {
        <<abstract>>
    }
    class AirPressurePoint {
        <<abstract>>
    }
    class AirPressureSensor {
        <<abstract>>
    }
    class AirPressureSp {
        <<abstract>>
    }
    class AirTempPoint {
        <<abstract>>
    }
    class AirTempSensor {
        <<abstract>>
    }
    class AirTempSp {
        <<abstract>>
    }
    class ZoneAirTempSp {
        <<abstract>>
    }
    class BoolPoint {
        <<abstract>>
    }
    class NumberPoint {
        <<abstract>>
    }
    class EnumPoint {
        <<abstract>>
    }
    class CmdPoint {
        <<abstract>>
    }
    class SensorPoint {
        <<abstract>>
    }
    class SpPoint {
        <<abstract>>
    }
    class ComputedSyntheticPoint {
        <<abstract>>
    }
    class MlSyntheticPoint {
        <<abstract>>
    }
    class SimSyntheticPoint {
        <<abstract>>
    }
    class Co2Point {
        <<abstract>>
    }
    class Co2Sensor {
        <<abstract>>
    }
    class Co2Sp {
        <<abstract>>
    }
    class DamperPoint {
        <<abstract>>
    }
    class DamperSensor {
        <<abstract>>
    }
    class DamperCmd {
        <<abstract>>
    }
    class ElecSensor {
        <<abstract>>
    }
    class ElecDemandSensor {
        <<abstract>>
    }
    class ElecEnergySensor {
        <<abstract>>
    }
    class ElecAcPfSensor {
        <<abstract>>
    }
    class ElecAcEnergySensor {
        <<abstract>>
    }
    class ElecAcActiveEnergySensor {
        <<abstract>>
    }
    class ElecAcReactiveEnergySensor {
        <<abstract>>
    }
    class ElecAcApparentEnergySensor {
        <<abstract>>
    }
    class ElecAcDemandSensor {
        <<abstract>>
    }
    class ElecAcPowerDemandSensor {
        <<abstract>>
    }
    class ElecAcActiveDemandSensor {
        <<abstract>>
    }
    class ElecAcReactiveDemandSensor {
        <<abstract>>
    }
    class ElecAcApparentDemandSensor {
        <<abstract>>
    }
    class FanPoint {
        <<abstract>>
    }
    class FanRunSensor {
        <<abstract>>
    }
    class FanRunCmd {
        <<abstract>>
    }
    class FanEnableSensor {
        <<abstract>>
    }
    class FanEnableCmd {
        <<abstract>>
    }
    class FanSpeedSensor {
        <<abstract>>
    }
    class FanSpeedCmd {
        <<abstract>>
    }
    class RunPoint {
        <<abstract>>
    }
    class RunSensor {
        <<abstract>>
    }
    class RunCmd {
        <<abstract>>
    }
    class EnablePoint {
        <<abstract>>
    }
    class EnableSensor {
        <<abstract>>
    }
    class EnableCmd {
        <<abstract>>
    }
    class AlarmSensor {
        <<abstract>>
    }
    class VfdFreqPoint {
        <<abstract>>
    }
    class VfdFreqSensor {
        <<abstract>>
    }
    class VfdFreqCmd {
        <<abstract>>
    }
    class VfdSpeedPoint {
        <<abstract>>
    }
    class VfdSpeedSensor {
        <<abstract>>
    }
    class VfdSpeedCmd {
        <<abstract>>
    }
    class NaturalGasFlowPoint {
        <<abstract>>
    }
    class NaturalGasVolumePoint {
        <<abstract>>
    }
    class NaturalGasEnergyPoint {
        <<abstract>>
    }
    class OccupiedPoint {
        <<abstract>>
    }
    class OccupiedSensor {
        <<abstract>>
    }
    class OccupiedSp {
        <<abstract>>
    }
    class ValvePoint {
        <<abstract>>
    }
    class ValveSensor {
        <<abstract>>
    }
    class ValveCmd {
        <<abstract>>
    }
    class WaterFlowPoint {
        <<abstract>>
    }
    class WaterFlowSensor {
        <<abstract>>
    }
    class WaterFlowSp {
        <<abstract>>
    }
    class WaterPressurePoint {
        <<abstract>>
    }
    class WaterPressureSensor {
        <<abstract>>
    }
    class WaterPressureSp {
        <<abstract>>
    }
    class WaterTempPoint {
        <<abstract>>
    }
    class WaterTempSensor {
        <<abstract>>
    }
    class WaterTempSp {
        <<abstract>>
    }
    class WaterVolumePoint {
        <<abstract>>
    }
    class WaterVolumeSensor {
        <<abstract>>
    }
    class WaterVolumeSp {
        <<abstract>>
    }
    class WeatherNumberPoint {
        <<abstract>>
    }
    class ElecDcCurrentSensor {
        <<abstract>>
    }
    class ElecDcPowerSensor {
        <<abstract>>
    }
    class ElecDcEnergySensor {
        <<abstract>>
    }
    class ElecVoltSensor {
        <<abstract>>
    }
    class ElecCurrentSensor {
        <<abstract>>
    }
    class ElecPowerSensor {
        <<abstract>>
    }
    class ElecAcVoltSensorX {
        <<abstract>>
    }
    class ElecAcMagnitudeVoltSensor {
        <<abstract>>
    }
    class ElecAcCurrentSensorX {
        <<abstract>>
    }
    class ElecAcMagnitudeCurrentSensor {
        <<abstract>>
    }
    class ElecAcAngleCurrentSensor {
        <<abstract>>
    }
    class ElecAcQualityCurrentSensor {
        <<abstract>>
    }
    class ElecAcCurrentDemandSensor {
        <<abstract>>
    }
    class ElecAcAvgMagnitudePowerSensor {
        <<abstract>>
    }
    class ElecAcActivePowerSensor {
        <<abstract>>
    }
    class ElecAcReactivePowerSensor {
        <<abstract>>
    }
    class ElecAcApparentPowerSensor {
        <<abstract>>
    }
    class ElecDcCurrentMaxSp {
        <<abstract>>
    }
    class ElecDcPowerMaxSp {
        <<abstract>>
    }
    class ElecSp {
        <<abstract>>
    }
    class ElecMaxSp {
        <<abstract>>
    }
    class ElecCurrentMaxSp {
        <<abstract>>
    }
    class ElecPowerMaxSp {
        <<abstract>>
    }
    class ElecDemandMaxSp {
        <<abstract>>
    }
    class ElecAcCurrentMaxSp {
        <<abstract>>
    }
    class ElecAcPowerMaxSp {
        <<abstract>>
    }
    class ElecAcMagnitudePowerMaxSp {
        <<abstract>>
    }
    class ElecAcActivePowerMaxSp {
        <<abstract>>
    }
    class ElecAcActiveDemandMaxSp {
        <<abstract>>
    }
    class FilterPoint {
        <<abstract>>
    }
    class FilterSensor {
        <<abstract>>
    }
    class FilterPressurePoint {
        <<abstract>>
    }
    class NaturalGasPressurePoint {
        <<abstract>>
    }
    class DateTimePoint {
        <<abstract>>
    }
    class PumpPoint {
        <<abstract>>
    }
    class PumpRunSensor {
        <<abstract>>
    }
    class PumpRunCmd {
        <<abstract>>
    }
    class PumpEnableSensor {
        <<abstract>>
    }
    class PumpEnableCmd {
        <<abstract>>
    }
    class PumpSpeedSensor {
        <<abstract>>
    }
    class PumpSpeedCmd {
        <<abstract>>
    }
    class SteamFlowPoint {
        <<abstract>>
    }
    class SteamPressurePoint {
        <<abstract>>
    }
    class SteamTempPoint {
        <<abstract>>
    }
    class SteamEnergyPoint {
        <<abstract>>
    }
    class ThermalEnergyPoint {
        <<abstract>>
    }
    class ThermalPowerPoint {
        <<abstract>>
    }
    class HpbsDischargeColor {
        <<abstract>>
    }
    class HpbsReturnColor {
        <<abstract>>
    }
    class HpbsZoneColor {
        <<abstract>>
    }
    class HpbsOutsideColor {
        <<abstract>>
    }
    class HpbsMixedColor {
        <<abstract>>
    }
    class HpbsExhaustColor {
        <<abstract>>
    }
    class HpbsInletColor {
        <<abstract>>
    }
    class HpbsSetpointColor {
        <<abstract>>
    }
    class HpbsHotWaterColor {
        <<abstract>>
    }
    class HpbsChilledWaterColor {
        <<abstract>>
    }
    class HpbsCondenserWaterColor {
        <<abstract>>
    }
    class HpbsDomesticHotWaterColor {
        <<abstract>>
    }
    class HpbsSteamColor {
        <<abstract>>
    }
    class HpbsGasColor {
        <<abstract>>
    }
    class HpbsElecColor {
        <<abstract>>
    }
    class HpbsSensorColor {
        <<abstract>>
    }
    class HpbsCommandColor {
        <<abstract>>
    }
```
