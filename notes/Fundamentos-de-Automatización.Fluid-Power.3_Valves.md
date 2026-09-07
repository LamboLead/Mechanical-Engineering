---
id: 8mhijg7di314uagzwaf9zgp
title: '3.1 - Valves'
desc: ''
updated: 1746416374649
created: 1746138084143
---

## Objectives

This section contains topics related to:
1. Valve applications, classification of directional control valves.
2. Bernoulli's equation: Calculate pressure at a certain point in a streamline, and calculate the pressure drop accross a valve at a given flow rate and orifice area.
3. Check valves: Explain how they, and pilot-operated check valves work, and design a hydraulic circuit using a check valve to bypass or lock a component.

---

## 1. Directional control valves

These are classified by:

- Number of flow paths/ways.
- Number of positions.
- Actuation method: Manual, solenoid, spring-return, pneumatic, hydraulic, etc.
- Center condition: Condition of the valve when it is on its default (center) position:
  
  ![](/assets/images/2025-05-01-17-32-30.png)

  **Examples:**
  
  - ![](/assets/images/2025-05-01-17-33-07.png) : 3-way, 2-position. Hydraulic actuation (by a hydraulic pilot).
  - ![](/assets/images/2025-05-01-17-33-57.png) : 4-way, 3-position. Lever actuation, spring-return.
  - ![](/assets/images/2025-05-01-17-34-56.png) : 5-way, 3-position. Solenoid actuation

## 2. Needle valves

These valves allow to regulate the speed of the circuit by regulating the pressure drop accross itself.

### Bernoulli's equation (conservation of energy)

This is an equation that describes the behaviour of flow when it is flowing through a conduit.

![](/assets/images/2025-05-01-17-38-57.png)

**Assumptions:**
- The fluid is incompressible.
- There is a steady-flow.
- The flow is frictionless between the conduit's surface and itself.
- Each point is on a streamline.

### Application of Bernoulli's equation to orifice-flow

Assume a situation in which a fluid is passing through a conduit and then through a small orifice.

**What happens with fluid flow after the orifice?**

![](/assets/images/2025-05-01-17-51-35.png)

**What is the pressure drop after the orifice?**

![](/assets/images/2025-05-01-17-54-05.png)

**Example:** Pressure drop accross a needle valve

![](/assets/images/2025-05-01-18-03-02.png)

Orifice coefficient ($K$): It is a coefficient that helps to calculate the amount of fluid flow according to the pressure drop on a needle valve, or viceversa.

## 3. One-way valve (Check-valve)

This valve allows fluid to pass from one way to another, but doesn't allow the fluid to return by the same path.

Internally, their architecture differs depending on the element that provides the seal between the two exits of the valve.

![](/assets/images/2025-05-03-15-15-11.png)

### Applications

1. **Car jack:** The check valves allow the user to have different pumping strokes to raise the car.

  ![](/assets/images/2025-05-03-15-19-39.png)

2. **Component bypass:** The use of a check valve on this circuit allows the flow to bypass the needle valve and allow full-speed extension, but slow retraction.

  ![](/assets/images/2025-05-03-15-41-27.png)

3. **Cylinder locking:** A check valve is used to maintain the pressure on the cylinder when the power is off. Also, a pilot-operated check valve can be used to return the circuit to the original state.

  ![](/assets/images/2025-05-03-16-33-23.png)