# Phase 2 Report  
Principles of Mechanical Design  

**Team Members:** Benjamin Givens, Isaac Rosas, Alex Wang  

---

# 1. Final Design Overview

## 1.1 System Description

The purpose of this mechanism is to deploy airbrake flaps to increase aerodynamic drag and control the descent of a rocket.

The system converts rotational motion from a servo motor into linear motion of airbrake flaps using a linkage mechanism.

The mechanism is a crank-slider system. The input is rotational torque, and the output is linear displacement of the airbrake flaps.

---

## 1.2 Major Components

(keep your existing text here — it’s good)

---

## 1.3 Changes from Phase 1

(keep your text)

---

# 2. CAD Model Development

## 2.1 Assembly Model

(keep your text)

---

## 2.2 Exploded View

(keep your text)

---

## 2.3 Motion Study

(keep your text)

---

## 2.4 Part Drawings

(keep your text)

---

# 3. Design for 3D Printing and Assembly

## 3.1 Printability

(keep your text)

---

## 3.2 Minimum Feature Sizes

(keep your text)

---

## 3.3 Assembly Considerations

(keep your text)

---

# 4. Engineering Analyses

## 4.1 Assumptions and Input Conditions

(keep your text)

---

## 4.2 Static Stress and Factor of Safety

**Component: Linkage Arm**

$$
\sigma = \frac{F}{A}
$$

$$
\sigma_b = \frac{F}{t d}
$$

Axial Stress Results  
Hand Calculation: 0.54467 MPa  
ANSYS Result: 0.53999 MPa  

Bearing Stress Results  
Hand Calculation: 1.702 MPa  
ANSYS Result: 1.7315 MPa  

$$
n = \frac{S_y}{\sigma}
$$

Yield Factor of Safety: 129.6  

### ANSYS Results

![Equivalent Stress](Equivalent%20Stress%20Linkage.png)

![Mid Axial Stress](Mid-Axial%20Stress%20Linkage.png)

![Bearing Stress](Bearing%20Stress%20Linkage.png)

---

## 4.3 Fatigue Assessment

$$
\sigma_a = \frac{\sigma_{max} - \sigma_{min}}{2}, \quad
\sigma_m = \frac{\sigma_{max} + \sigma_{min}}{2}
$$

$$
n = \frac{S_f}{\sigma_a}
$$

Linkage Fatigue FOS: 45.3  
Pin Fatigue FOS: 41.1  

![Fatigue Linkage](Fatigue%20Life%20Linkage.png)

![Bolt Fatigue](Bolt%20Fatigue%20Life.png)

---

## 4.4 Interface Stress Analysis

$$
\tau = \frac{F}{A}
$$

Hand Calculation: 1.3545 MPa  
ANSYS Result: 1.361 MPa  

![Bolt Shear](Bolt%20Shear%20Stress.png)

![Dowel Pin](Dowel%20Pins%20in%20Air%20Flap.png)

![Dowel Pin Fatigue](Bolt%20Fatigue%20Life.png)

---

## 4.5 Bearing Load Check

The shaft is supported by two bearings which react the applied load from the linkage system. Assuming the total applied load of 14.51 N is evenly distributed, each bearing experiences approximately 7.25 N.

This load is significantly lower than typical bearing capacity values, which are on the order of hundreds to thousands of newtons. Therefore, the bearings are expected to operate well within safe limits.

---

# 5. Global Safety Overview

Linkage Arm — Yielding — 129.6  
Linkage Arm — Fatigue — 45.3  
Pin (Bolt) — Shear Yield — 117.6  
Pin (Bolt) — Fatigue — 41.1  

The linkage arm experiences the highest stress; however, all components exhibit extremely high safety margins.

The system is structurally safe and highly over-designed for the given loading conditions.

---

# 6. Design Risks and Weaknesses

(keep your section — it's strong)

---

# 7. Conclusion

The final design consists of eight primary components and successfully converts rotational motion into controlled linear motion.

The analysis demonstrates high factors of safety in both static and fatigue loading.

The design meets all project requirements and is expected to perform reliably.

---

# 8. References

Norton, R. L. (2019). *Design of Machinery*  

MatWeb – 6061 Aluminum Properties  

---

# 9. Appendix

(keep your list)
