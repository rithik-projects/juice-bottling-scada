This project is a complete industrial automation simulation of a juice bottling plant developed using Ignition SCADA (Perspective Module).
It demonstrates real-time monitoring, control logic, safety interlocks, alarm handling, and process visualization.

The system mimics a real production line including mixing, filling, and bottling operations.

Key Features:

Process Automation:
Step-based sequence control (Idle → Check → Mixing → Filling)
Automatic cycle operation
Timer-based process simulation

 Safety System:
Emergency Stop (E-Stop) logic
Safety interlocks based on tank levels
System auto-shutdown on unsafe conditions


 HMI Dashboard (Perspective):
Real-time system status (RUNNING / STOPPED)
Safety indicator (SAFE / NOT SAFE)
Tank level visualization (Water, Juice, Mixing Tank)
Bottle production counter
Interactive START / STOP / RESET controls


 Tank & Process Simulation:
Mixing tank fill and drain animation
Water and juice consumption during production
Dynamic level updates


 Alarm System:
Low Water Alarm (< 35%)
Low Juice Alarm (< 35%)
Visual alarm indicators on HMI


 Equipment Simulation:
Mixing motor logic
Filling system operation
Conveyor concept (expandable)


System Architecture:

JuicePlant
├── Controls (Start, Stop, EStop, SafetyOK, SystemRunning)
├── Process (WaterLevel, JuiceLevel)
├── Equipment (MixingTank, Bottles, Pumps)
├── Simulation (ProcessStep, Timers)
└── Alarms (LowWater, LowJuice)


How It Works:
*Operator presses START
*System checks safety conditions
*Mixing tank fills and mixes
*Bottles are filled
*Water & juice levels decrease
*Cycle repeats automatically
*Alarms trigger if levels are low
