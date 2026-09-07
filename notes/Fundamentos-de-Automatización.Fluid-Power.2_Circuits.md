---
id: 0x6xg5fw6hy16g3hh4v0hnj
title: 2_Circuits
desc: ''
updated: 1746137929132
created: 1745262538764
---

Here, the fundamentals of fluid power circuits are shown:

## Components

### Line types

![Diagram with three types of lines: Pressure, return and control lines](/assets/images/2025-04-21-14-10-09.png)

- **Pressure lines:** Represented by continous lines. These lines are the ones that fluid pass though with high pressure on the circuit.
- **Return lines:** Represented by dashed lines that go to the reservoir. These allow the fluid to return to the reservoir in certain conditions.
- **Control lines:** Represented by dashed lines that go to certain componentes. These allow to control the actuation of a certain component when a certain condition is met.

### The cylinder

![](/assets/images/2025-04-21-14-11-32.png)

Each cylinder has two ports to allow the fluid to enter or leave when the piston is moved.

### Rotating components

These are pumps, regulated pumps, axle-powered pups, and pumps with returns. These can also be fluid power motors.

### Valves

**Válvula de alivio de presión:** Permite limitar la presión del sistema.
![](/assets/images/2025-04-21-14-16-46.png)

**Válvula de control direccional:** La posición central es aquella que la válvula tiene por defecto.
![](/assets/images/2025-04-21-14-21-29.png)

## Circuit conduits

These are lines or pipes (flexible or rigid) to transport the pressurized fluid to different elements of the fluid circuit

The conduits offer quite a lot of resistance to the flow, ussually related to fluid viscosity and it adhering to the inner surface of the hose, and losses related to turbulance in the fittings.

Some hose rated pressures: 3000psi or 21MPa, 65000psi or 450bar.

### Fluid viscosity

Ressistance of a fluid to flow. Is the ratio of shear-stress to the velocity-gradient.

![](/assets/images/2025-04-22-21-25-16.png)

In hydraluics, the fluids used are newtonian.

Unit: Pascal.second. Centipoise [cP] = 1 milliPascal.s


**Kinematic viscosity:** How the fluid will flow under the influence of gravity.

$v = \frac{\mu}{\rho} \space [cSt]$

Centistoke: $cSt = 10^{-6} m^2/s$

In hydraulic oils, the kinematic viscosity is around 20-70cSt.

> There is no ideal viscosity, because it is a trade-off:
>
> ![](/assets/images/2025-04-22-21-31-57.png)

Viscosity changes with temperature.

**Viscosity index:** It is a dimensionless number that quantifies the change in viscosity of a fluid around different temperatures.

### Pressure drop in pipes

For a fluid to flow there must be a pressure difference between two points.

There are two types of flow:
- Laminar: Gradual changes in geometry or diameter.
- Turbulent: High-velocity or large changes in geometry.

**Reynolds Number:** Relationship between inertial forces and viscous forces of the fluid. it helps classify the type of flow.

![](/assets/images/2025-04-22-22-23-15.png)

**Pressure drop in pipes:**

![](/assets/images/2025-04-22-22-25-52.png)

The moody diagram helps you get the friction factor according to the Reynolds Number and the roughness of the pipe.

![](/assets/images/2025-04-22-22-27-48.png)

**Pressure drop in pipes, laminar flow:**

![](/assets/images/2025-04-22-22-28-52.png)

**Exercise:** 3 Mega Watt wind turbine

![](/assets/images/2025-04-22-22-34-58.png)

### Pressure drop in fittings

**Hydraulic fittings**

![](/assets/images/2025-04-22-22-37-15.png)

The loss coefficient is related to the geometry, roughness and overall length of the fitting itself.

---

## Questions:

1. Why does the friction factor decrease with increasing Reynolds number? Why does the friction factor become independent of the Reynolds number as the relative roughness increases? Why is the friction factor independent of relative roughness in the laminar regime? Can you observe any other patterns?

  **Ans:**
  
  **The friction factor decreases with increasing Reynolds number** because because as the flow becomes more turbulent, the interactions between the flow and the inner surface of the pipe become less prevalent (because the boundary layer of the fluid becomes smaller), thus reducing the overall friction between the flow and the pipe.

  **The friction factor becomes independent of the Reynolds number as the relative roughnes increases** because when relative roughness is higher, the surface peaks have more influence over the friction flow than the flow's viscous forces themselves. This flow state is called _rough turbulent_.

  **The friction factor is independent of any relative roughness in the laminar regime** because in laminar flow, the flow follows predictable layers; for example, at the surface of the pipe, the flow velocity is zero, so surface roughness has almost no effect on the flow regarding friction.

2. What are some general rules of thumb for plumbing efficient fluid power systems?

  **Ans:**
   - Minimize fittings. Each fitting adds pressure drop; use smooth bends over sharp elbows.
   - Use larger diameter pipes to reduce velocity and friction losses.
   - Avoid sudden changes in direction or diameter, these cause turbulence and energy loss.
   - Keep pipe runs short and straight to reduce total friction resistance.
   - Select fittings with low loss coefficients, Especially in high-flow sections.
   - Match pipe size to flow rate: Oversizing implies more piping cost, and undersizing wastes energy.