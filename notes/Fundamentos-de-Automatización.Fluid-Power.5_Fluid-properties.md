---
id: 2z2lwljhy5zgkjpx67zktr0
title: '5 - Fluid properties'
desc: ''
updated: 1746586958145
created: 1746576673835
---

## Objectives

This section contains topics related to:

1. Fluid properties: Importance of fluid properties, fluid additives
2. Fluid Compressibility and inertia: Calculation, importance and related equations.

---

## Fluid additives

The role of hydraulic fluid is:

- Transmission of power (primary)
- Lubrication between components
- Sealing between components
- Heat transfer/cooling

The most important fluid properties:

**Primary:**

- Viscosity: Flow resistance
- Bulk modulus: Matters for compresibility
- Density: Matters for mass and inertia

**Secondary:**
- Heat capacity, to reduce its thermal inertia.
- Vapor pressure, to know at which point the fluid will cavitate.
- Lubricity: To maintain boundary lubrication
- Flash point, to avoid a fire hazard
- Oxidation, to avoid oil breakdown.
- Foaming, to allow release of air

### Hydraulic oil additives

**Mineral oil additives:**

- Oxidation and corrosion resistance.
- Foaming reduction.
- Lubricity
- High viscosity index.

**Fire resistant fluids**
- Oil/water emulsions

## Fluid compressibility

Hydraulic fluid is compressible, and the compressilibity of a fluid is described thorugh the bulk modulus $\beta$

**Bulk modulus:** Id describes the pressure required to cause a given volume of fluid by a certain amount.

$$
\beta = \frac{-dP}{dV/V}
$$

Usually, hydraulic oils range from a bulk modulus of 1.5 to 1.9 GPa (around 1% to 5%), while that of water is about 2.2GPa. Also, the bulk modulus is dependent of pressure.

### Importance of compressibility

Compressibility can be important when the hydraulic actuator needs to hold something heavy, with precise positioning. Also, it can lead to energy losses when the circuit needs to compress the fluid and then it is released, wasting that energy.

## Cylinder resonance

![](/assets/images/2025-05-06-20-21-48.png)

**Example:** Calculate the resonant frequency of a cylinder described below.

![](/assets/images/2025-05-06-20-23-19.png)

## Fluid inertia

When a fluid is passing through a pipe, and the flow is suddenly interrupted by a fast-closing valve, the internal components of the pipe experience a water hammer, which is a byproduct of fluid inertia.

**Innertial pressure:** $\Delta P = \frac{\rho L}{A}\frac{dQ}{dt}$

**Calculating inertia for a flowing fluid through a pipe:**

![](/assets/images/2025-05-06-21-58-31.png)

**Example:** Water hammer at a faucet. What is the pressure that the system experiences when a faucet is closed in 10 milliseconds?

![](/assets/images/2025-05-06-22-01-42.png)