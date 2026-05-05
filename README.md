# ⚙️ 4-Speed Manual Gearbox Project
### *Inspired by the Getrag MMT6 (Ford Mondeo MK4 2.0 TDCi)*

---

## Project Overview
This project involves the design and functional simulation of a 4-speed manual transmission in Autodesk Fusion 360. The gear geometry and ratios are modeled after the first four speeds of the **Getrag MMT6** transaxle, found in the 2008 Ford Mondeo MK4 2.0 TDCi.

---

## Technical Specifications
| Component | Specification |
| :--- | :--- |
| **Gear Type** | Spur (for high torque & low noise) |
| **Reference Gearbox** | Getrag MMT6 (6-Speed Manual) |
| **Output Shaft** | 15mm Hexagonal |
| **Shifting Mechanism** | Sliding Dog Clutch |

---

## Gear Ratio Data (MMT6 2.0 TDCi)
To maintain authenticity, the model utilizes the factory ratios of the Ford Mondeo MK4.

| Gear | Ratio | Tooth Count Example (Approximated) |
| :--- | :--- | :--- |
| **1st Gear** | **3.231 : 1** | 13T Driver / 42T Driven |
| **2nd Gear** | **1.952 : 1** | 21T Driver / 41T Driven |
| **3rd Gear** | **1.321 : 1** | 28T Driver / 37T Driven |
| **4th Gear** | **1.029 : 1** | 32T Driver / 33T Driven |

---

## Design Methodology
The design uses a **Constant Mesh** architecture where all gear pairs are always engaged, and power is transferred only when the dog clutch locks a gear to the mainshaft.

### Modeling Process in Fusion 360
*   **Joints & Motion Links:** 
    *   **Revolute Joints** for the input and layshafts.
    *   **Motion Links** applied to simulate the MMT6 ratios (e.g., for 1st gear, the link is set at $1 / 3.231$).

---

## Assembly Breakdown
### Main Components
1.  **Input Shaft:** Transfers power from the simulated 2.0 TDCi flywheel.
2.  **Layshaft (Countershaft):** Forges the mechanical link between the input and the mainshaft gears.
3.  **Mainshaft (Output):** Features the four driven gears.
