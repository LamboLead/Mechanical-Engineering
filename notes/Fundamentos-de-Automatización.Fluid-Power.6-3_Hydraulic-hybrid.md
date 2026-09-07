---
id: tbiz7f3ua43251nmjemtxi4
title: "6.3 - Hydraulic-hybrid vehicles"
desc: ''
updated: 1747023139710
created: 1747014976849
---

## Objectives

This section contains topics related to:

1. Hydraulic hybrid vehicles: Applications, benefits and limitations.
2. Hydraulic hybrid architectures: Architecture configurations (parallel, series and split), benefits and limitations.
3. Component sizing, simulation and interactions between components.

---

## Why to hybridize a power train?

- To recapture the kinetic energy during braking.
- To turn off the engine when stopped.
- To run the IC engine at peak efficiency and peak power.

**Hydraulic vs. electric hybrid:**

![](/assets/images/2025-05-11-21-03-28.png)

The best applications for hydraulic hybrid vehicles, are large vehicles who have lots of space and are not restricted by weight and high-accelerations.

## Hydraulic hybrid architectures

**Parallel:** The existing mechanical drivetrain is retained, and the pump/motor are coupled co-axially to the drive shaft. These allow to store some energy in form of fluid energy to assist the IC engine, but the engine is not decoupled to the road load.

![](/assets/images/2025-05-11-21-14-42.png)

**Series:** It has a fully hydraulic transmission, so the engine load is decoupled from the road load, and the engine off operation is possible (70% improvement in fuel economy, and 40% reduction in CO2 emmissions.).

All of the power from the engine is sent through the hydraulic transmission, thus not reaching full efficiencies.

![](/assets/images/2025-05-11-21-15-26.png)

![](/assets/images/2025-05-11-21-19-22.png)

**Power split:** There are two power paths, with a high-efficiency path through a mechanical transmission, and infinte speed variability through a hydraulic transmission.

![](/assets/images/2025-05-11-21-25-42.png)

![](/assets/images/2025-05-11-21-25-59.png)

## Component sizing for hydraulic hybrid vehicle

Consider a passenger car with the following specs. Size the pump, accumulator and motor-pump to implement a hydraulic hybrid system in series for the vehicle.

![](/assets/images/2025-05-11-22-45-11.png)

### Sizing the accumulator

Calculate the size (volume) of the accumulator in the hydraulic hybrid system for said specifications.

**Assumptions:**
- It will be sized for every 20m/s braking event.
- Gas will actuate isothermally.
- 2:1 pressure ratio.
- Maximum pressure will be 35MPa.
- Neglect inefficiencies.

![](/assets/images/2025-05-11-22-50-57.png)

### Sizing the motor-pump

Calculate the size (power and speed) of the motor-pump in the system.

**Assumptions:**
- The peak acceleration of the vehicle is $1.5m/s^2$
- Direct drive a single wheel.
- Peak power will be achieved at minimum pressure.
- Neglect road loads and inefficiencies.

![](/assets/images/2025-05-11-22-55-42.png)

### Sizing the pump

Calculate the size (pressure, flow rate, and power) for the pump of the system.

**Assumptions:**
- The IC engine will be treated as on-off based on accumulator pressure.
- On condition will be most efficient for the IC engine.
- The sizing of the pump will be done for road loads (drag and rolling ressistance) af maximum speed (25m/s).
- Neglect inertial force
- Neglect inefficiencies.

![](/assets/images/2025-05-11-23-12-18.png)