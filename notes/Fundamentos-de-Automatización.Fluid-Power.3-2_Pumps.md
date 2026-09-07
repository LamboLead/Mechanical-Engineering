---
id: avts20j98wsptprmhx8a4mx
title: '3.2 - Pumps'
desc: ''
updated: 1746416443530
created: 1746328913103
---

## Objectives

This section contains topics related to:
1. Component explanation and applications. Positive and non-positive displacement pumps, and physical variables related to their working.
2. Pumps library: Common hydraulic pump architectures, benefits and limitations.
3. Pump ripple: Explanation and appearance in parameter gear or piston pump.
4. Pump efficiency: Forms of energy loss and calculation of a hydraulic pump
5. Pump power supply: Role of primary components, direct-acting/pilot-operated pressure relief valve.
6. Pump action: Hydraulic pump and motor, speed and torque relationships.

---

## Introduction to pumps

There are two types of hydraulic fluid pumps:

### Positive displacement pumps

These pumps circulates a certain amount of volume per revolution. Their flow rate is kinematics-dependent, and their equations are:

  **Flow rate:** $Q=\frac{D\omega}{2\pi} \space[m^3/s]$   
  **Torque:** $T=\frac{DP}{2\pi} \space [N.m]$

  With:
  - $D$: Displacement $[m^3/rev]$
  - $P$: Pressure
  - $\omega$: Revolutions per second.

![Schematic of a positive displacement pump](/assets/images/2025-05-03-17-26-09.png)

**Applications:** Low-velocity, low-flow rate, high-force applications; like a log-splitter.

> If the outlet is blocked and the pressure in the system increases, a positive displacement pump can be stalled. To avoid this, a relief-valve must be used in parallel with the pump.

### Non-positive displacement pumps

These pumps work continuously by rotating an impeller. Their flow rate is pressure-dependent.

![Schematic of a non-positive displavement pump](/assets/images/2025-05-03-17-26-31.png)

**Applications:** High-velocity, high-flow rate, low-power-applications.

> If the outlet is blocked, a non-positive displacement pump won't stall.

### Two-stage pumps

These are pumps that increase the pressure of a system when a high-velocity and flow-rate is needed in combination with high-force.

![Schematic of a two-stage pump inside a log-splitter. The high-pressure pump is activated when the unloading valve's pressure is surpassed in the circuit, while the low-presure pump flow is returned to the reservoir](/assets/images/2025-05-03-17-09-03.png)

## Pump architectures

### Gear pumps

- Fixed displacement
- Inexpensive: Only two moving parts.
- Positive displacement
- Low efficiency: High points of leakage.
- Loud: High-ripple
- Limited pressure.

![](/assets/images/2025-05-03-17-28-22.png)

### Vane pumps

- Fixed/variable displacement.
- Quiet: Less flow-ripple.
- Limited pressure.
- Self-adjusting: As they wear-out, the veins stick out automatically due to fluid pressure.

![Schematic of a vane pump](/assets/images/2025-05-03-17-31-09.png)

### Piston pumps

- High-efficiency.
- Fixed/variable displacement.
- Very high pressures.
- More durable: Pumping fluid is separate from the case.

1. **Inline piston:** Piston pumps composed of only one piston. These are capable of high pressures and are of fixed displacement.
   
   ![Image of an inline piston pump](/assets/images/2025-05-03-21-57-35.png)

1. **Radial piston:** These have their pistons oriented radially, and an eccentric shaft is designed with lobes on it to move the pistons. They can be single/multi-lobed, fixed/variable displacement, and are more compact than other designs.
   
  ![Schematic of single-lobed radial piston pump](/assets/images/2025-05-03-22-00-03.png)

  ![Schematic of a pancake-architecture hollow-shaft radial piston pump](/assets/images/2025-05-03-22-00-19.png)

3. **Axial piston:** These are divided in:
   1. **Swash-plate:** This is a compact, and fixed/variable displacement.
   
   ![](/assets/images/2025-05-03-22-10-43.png)
   
   2. **Bent-axis:** This is a high-efficiency, high-offset angle, fixed/variable displacement, but expensive pump.
   
   ![](/assets/images/2025-05-03-22-10-02.png)

## Flow-ripple

Flow-ripple is the variation of the flow rate of a pump due to the geometry and kinematics of the pump. It causes vibrations and noise in the system.

![](/assets/images/2025-05-03-21-30-01.png)

**Flow-ripple on piston pumps:** Here is the flow-ripple graph amount depending on the number of pistons in the pump:

![](/assets/images/2025-05-03-21-32-46.png)

## Pumping efficiency

There are multiple sources of energy loss on a piston pump:

- Piston-cylinder interface due to leakage or viscous friction.
- Bearing friction (hydrostatic, simple, roller).
- Seal friction
- Fluid compressibility
- Internal valves: Throttling, leakage and friction.

### Energy loss on piston-cylinder interface

![](/assets/images/2025-05-03-22-57-35.png)

By plotting the corresponding equations on MatLab, the following graph is created:

![Clearance and Piston length vs. Energy loss chart for a single-piston pump by leakage](/assets/images/2025-05-03-23-02-02.png)

This means that, the pump manufacturer can choose a certain clearance to manufacture the cylinders and pistons, and then select the piston length that minimizes the energy loss.

**How to model pump efficiency?**

![](/assets/images/2025-05-03-23-06-23.png)

## Hydraulic power supply

A hydraulic power supply is the assembly of components that allow the hydraulic circuit to generate power.

![](/assets/images/2025-05-03-23-09-14.png)

- **Reservoir:** This is the tank that contains the hydraulic fluid. It not only contains the fluid but also removes heat from it, a breather to allow the oil to depressurize, a sight gauge to check for fluid level, and magnetic drain plugs to catch metallic particles.

  ![](/assets/images/2025-05-03-23-11-09.png)

- **Filtration systems:** These components filter particles in the hydraulic fluid. It is very important to avoid wear between the surfaces of the componentes of the hydraulic circuit.

  ![](/assets/images/2025-05-03-23-15-47.png)

  > The application of different kinds of filters depends on the components being used at the circuit. If they can be easily damaged by different particles, you should use a multistage and high-quality filtration system.

- **Pressure regulation:** This function can be fulfilled by a needle valve, that returns fluid to the reservoir when the pressure at the fluid exceeds its setting.
  
  ![Schematic of a direct-acting pressure relief valve](/assets/images/2025-05-03-23-26-04.png)

  The pilot-operated pressure relief valve  

  ![Schematic of a pilot-operated pressure relief valve](/assets/images/2025-05-03-23-29-37.png)

### Hydrostatic transmission

A hydraulic motor is a rotational device that converts hydraulic energy into rotational mechanical energy.

![Symbols of a pump and a hydraulic motor](/assets/images/2025-05-04-18-53-39.png)

**Open hydrostatic motor:** It is a hydraulic circuit that integrates an axle-driven variable pump, a pressure relief valve, and a fixed hydraulic motor that drives another axle. It allows to create different gear-ratios.

![](/assets/images/2025-05-04-18-56-37.png)

**Closed hydrostatic motor:** It uses basically the same components as the open hydrostatic motor, but the pump is an 'over-center' variable pump (which means it can deliver pressure to both sides) and a bi-directional fixed motor; and having a pressure-relief valve for each flow direction (forward/reverse).

![](/assets/images/2025-05-04-19-02-46.png)

To account for the leakage for the more complex components, a 'charging circuit' is installed. It is composed of another pump, driven by the same axle as the main pump, to make for the lost pressure.

![](/assets/images/2025-05-04-19-04-27.png)

To integrate filtration on this system, a 'shutter-valve' is applied in parallel before the hydraulic motor, which is solenoid-activated by a sensor input or the user.

![](/assets/images/2025-05-04-19-05-41.png)