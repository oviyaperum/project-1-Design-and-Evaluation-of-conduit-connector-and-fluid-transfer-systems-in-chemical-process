# Design and Development of Conduit Connector Clips as an Innovative Alternative to Solid Connectors

## Report: OVIYA P (SAVEETHA ENGINEERING COLLEGE)

This project explores the application of **Additive Manufacturing (AM)**, specifically **Fused Deposition Modeling (FDM)**, to design and evaluate a custom conduit connector for low-pressure fluid transfer systems in chemical process industries. This addresses the challenge of acquiring customized or small-batch components where traditional methods are economically unviable.

The resulting 3D-printed connector offers a rapid, cost-effective solution for producing custom process components, especially for educational and prototyping needs.

## Key Objectives

1.  To design a 3D-printable conduit connector with industry-relevant geometry using **CAD tools**.
2.  To fabricate the connector using FDM with **PLA filament** and optimize printing parameters.
3.  To analyze mechanical and chemical performance through dimensional testing and flow experiments.
4.  To validate connector functionality through fluid dynamics calculations (e.g., head loss, Reynolds number).
5.  To propose improvements for scaling the solution for various fluid types and system pressures.

## 🛠️ Methodology & Materials

### Design and Modeling

* **Tool:** Autodesk Fusion 360 was used to model the conduit connector.
* **Design Specifications:** The model featured a cylindrical body with a **10 mm internal diameter**, press-fit grooves for tubing insertion, reinforcement collars, and chamfers at inlets to reduce flow turbulence.
* **Fabrication Method:** Fused Deposition Modeling (FDM) was chosen for its accessibility and cost-effectiveness.

### Material Selection: PLA

**Polylactic Acid (PLA)** was selected for this project due to its biodegradability, stiffness, dimensional accuracy, and low warping behavior during printing.

| Property | Value |
| :--- | :--- |
| **Density** | $1.24 \text{ g/cm}^3$ |
| **Tensile Strength** | $60 \text{ MPa}$ |
| **Chemical Compatibility** | Suitable for Water, alcohol, saline. |
| **Chemical Limitations** | Not suitable for acids, bases, or solvents. |

### Slicing and Printing Parameters

The STL file was imported into Ultimaker Cura for slicing.

| Parameter | Value |
| :--- | :--- |
| **Layer Height** | $0.2 \text{ mm}$ |
| **Wall Thickness** | $1.2 \text{ mm}$ (Three perimeters) |
| **Infill Pattern** | Grid ($25\%$) |
| **Nozzle Temperature** | $200 \text{ °C}$ |
| **Bed Temperature** | $60 \text{ °C}$ |

## 🧪 Results and Validation

### 1. Dimensional Analysis

Most deviations were **< $\pm 2 \%$**, which is well within the acceptable tolerance for lab-scale plastic components.

| Parameter | CAD (mm) | Printed (mm) | % Error |
| :--- | :--- | :--- | :--- |
| Internal bore diameter | $10.00$ | $9.82$ | $-1.8 \%$ |
| Total length | $65.00$ | $64.70$ | $-0.46 \%$ |

### 2. Hydraulic Performance

Testing in a $10 \text{ mm}$ ID PVC tubing circuit with water flow validated the design for practical use.

* **Maximum Flow Tested:** $2.54 \text{ L/min}$ (Turbulent regime: $Re = 6053$).
* **Head Loss:** At a typical loop flowrate of $1.72 \text{ L/min}$ (required for a $1.2 \text{ kW}$ cooling duty), the added head loss was **$4.4 \text{ mm}$ of water**.
* **Pump Impact:** This minuscule head loss translates to a pressure drop of **$43 \text{ Pa}$**, which is **negligible** ($< 0.002 \%$ of cooling-water pump rating).

### 3. Mechanical Integrity

* **Hoop Stress:** The calculated hoop stress was $0.6 \text{ MPa}$ for a worst-case design pressure of $0.3 \text{ MPa}$.
* **Safety Factor:** The estimated Safety Factor was **$> 50$** (relative to PLA ultimate tensile strength of $60 \text{ MPa}$).
* **Burst Test:** The connector successfully withstood a hydrostatic burst pressure of **$0.45 \text{ MPa}$**.

### 4. Chemical Compatibility

| Medium | Observation | Conclusion |
| :--- | :--- | :--- |
| Distilled water ($25 \text{ °C}$) | No change | **Suitable** for neutral aqueous streams. |
| $20 \%$ Ethanol | Slight surface whitening | **Limited Suitability** for solvents. |
| $2 \text{ M HCl}$ | Surface crazing after $3 \text{ h}$ | **Not Suitable** for strong acids. |

## 🚀 Design Improvements and Scale-Up

To extend the utility of the connector for industrial or more demanding lab environments:

1.  **Material Shift:** Upgrade to **PETG** or **Polypropylene (PP)** for better chemical resistance and a higher glass transition temperature ($80 \text{ °C}$ for PETG).
2.  **Pressure Rating:** Integrate a $1.5 \text{ mm}$ **O-Ring Groove** to embed an elastomer seal, potentially raising the pressure rating to $0.6 \text{ MPa}$.
3.  **Connectivity:** Implement **ISO 7/1 BSP threads** for compatibility with standard metal piping systems.

## Repository Guide

| File/Folder | Content Description |
| :--- | :--- |
| `README.md` | This project overview and summary of findings. |
| `documentation/` | Full **Mini Project Report** PDF. |
| `printing_files/` | Configuration file detailing the optimized **FDM settings**. |
| `cad/` | **Manufacturing Files (.STL, .STEP) for the DN32 Connector Components:** |
| `cad/STL/` | - [`conduit_connector_dn32_clips_x1_v7.stl`](cad/STL/conduit_connector_dn32_clips_x1_v7.stl) |
| | - [`conduit_connector_dn32_clip_locks_x1_v7.stl`](cad/STL/conduit_connector_dn32_clip_locks_x1_v7.stl) |
| | - [`conduit_connector_dn32_align_protrusions_x2_v3.stl`](cad/STL/conduit_connector_dn32_align_protrusions_x2_v3.stl) |
| `cad/STEP/` | - [`conduit_connector_dn32_clips_x1_v7.step`](cad/STEP/conduit_connector_dn32_clips_x1_v7.step) |
| | - [`conduit_connector_dn32_clip_locks_x1_v7.step`](cad/STEP/conduit_connector_dn32_clip_locks_x1_v7.step) |
| | - [`conduit_connector_dn32_align_protrusions_x2_v3.step`](cad/STEP/conduit_connector_dn32_align_protrusions_x2_v3.step) |

# FDM Optimized Slicing Parameters for PLA Connector
# Software: Ultimaker Cura (or equivalent)
# Reference: Project Report (Table 3.2)

[Machine & Material]
Material: Polylactic Acid (PLA), 1.75 mm diameter
Nozzle Diameter: 0.4 mm (Assumed standard)
Nozzle Temperature: 200 C
Bed Temperature: 60 C

[Quality]
Layer Height: 0.2 mm

[Shell]
Wall Thickness: 1.2 mm (Typically 3 perimeters for 0.4mm nozzle)

[Infill]
Infill Density: 25%
Infill Pattern: Grid

[Speed]
Print Speed: 50 mm/s

[Support]
Support Structure: Removed carefully after printing

[Post-Processing]
Sanding: Used 400-grit sandpaper for smoothness and tolerance matching
