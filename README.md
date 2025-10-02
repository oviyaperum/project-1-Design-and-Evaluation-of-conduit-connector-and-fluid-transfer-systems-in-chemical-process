# 3D-Printed Conduit Connector for Chemical Process Fluid Systems

##  Project Report: OVIYA P (212222210019)

[cite_start]This project explores the application of **Additive Manufacturing (AM)**, specifically **Fused Deposition Modeling (FDM)** [cite: 88, 107][cite_start], to design and evaluate a custom conduit connector for low-pressure fluid transfer systems in chemical process industries[cite: 6]. [cite_start]This addresses the challenge of acquiring customized or small-batch components where traditional methods are economically unviable[cite: 93, 94].

[cite_start]The resulting 3D-printed connector offers a rapid, cost-effective solution for producing custom process components, especially for educational and prototyping needs[cite: 46].

## [cite_start]Key Objectives [cite: 99, 100, 101, 102, 103]

1.  [cite_start]To design a 3D-printable conduit connector with industry-relevant geometry using **CAD tools**[cite: 99].
2.  [cite_start]To fabricate the connector using FDM with **PLA filament** and optimize printing parameters[cite: 100].
3.  [cite_start]To analyze mechanical and chemical performance through dimensional testing and flow experiments[cite: 101].
4.  [cite_start]To validate connector functionality through fluid dynamics calculations (e.g., head loss, Reynolds number)[cite: 102].
5.  [cite_start]To propose improvements for scaling the solution for various fluid types and system pressures[cite: 103].

## 🛠️ Methodology & Materials

### Design and Modeling

* [cite_start]**Tool:** Autodesk Fusion 360 was used to model the conduit connector[cite: 41, 115].
* [cite_start]**Design Specifications:** The model featured a cylindrical body with a **10 mm internal diameter** [cite: 42, 115][cite_start], press-fit grooves for tubing insertion, reinforcement collars, and chamfers at inlets to reduce flow turbulence[cite: 42, 115].
* [cite_start]**Fabrication Method:** Fused Deposition Modeling (FDM) was chosen for its accessibility and cost-effectiveness[cite: 41, 107].

### Material Selection: PLA

[cite_start]**Polylactic Acid (PLA)** was selected for this project due to its biodegradability, stiffness, dimensional accuracy, and low warping behavior during printing[cite: 116].

| Property | Value |
| :--- | :--- |
| **Density** | [cite_start]$1.24 \text{ g/cm}^3$ [cite: 116] |
| **Tensile Strength** | [cite_start]$60 \text{ MPa}$ [cite: 116] |
| **Chemical Compatibility** | [cite_start]Suitable for Water, alcohol, saline[cite: 116]. |
| **Chemical Limitations** | [cite_start]Not suitable for acids, bases, or solvents[cite: 116]. |

### Slicing and Printing Parameters

[cite_start]The STL file was imported into Ultimaker Cura for slicing[cite: 117].

| Parameter | Value |
| :--- | :--- |
| **Layer Height** | [cite_start]$0.2 \text{ mm}$ [cite: 117] |
| **Wall Thickness** | [cite_start]$1.2 \text{ mm}$ (Three perimeters) [cite: 117, 165] |
| **Infill Pattern** | [cite_start]Grid ($25\%$) [cite: 117, 165] |
| **Nozzle Temperature** | [cite_start]$200 \text{ °C}$ [cite: 117] |
| **Bed Temperature** | [cite_start]$60 \text{ °C}$ [cite: 117] |

## 🧪 Results and Validation

### 1. Dimensional Analysis

[cite_start]Most deviations were **< $\pm 2 \%$**, which is well within the acceptable tolerance for lab-scale plastic components[cite: 128, 129].

| Parameter | CAD (mm) | Printed (mm) | % Error |
| :--- | :--- | :--- | :--- |
| Internal bore diameter | [cite_start]$10.00$ [cite: 126] | [cite_start]$9.82$ [cite: 126] | [cite_start]$-1.8 \%$ [cite: 126] |
| Total length | [cite_start]$65.00$ [cite: 126] | [cite_start]$64.70$ [cite: 126] | [cite_start]$-0.46 \%$ [cite: 126] |

### 2. Hydraulic Performance

[cite_start]Testing in a $10 \text{ mm}$ ID PVC tubing circuit with water flow validated the design for practical use[cite: 131, 171].

* [cite_start]**Maximum Flow Tested:** $2.54 \text{ L/min}$ (Turbulent regime: $Re = 6053$)[cite: 132, 133].
* [cite_start]**Head Loss:** At a typical loop flowrate of $1.72 \text{ L/min}$ (required for a $1.2 \text{ kW}$ cooling duty) [cite: 154][cite_start], the added head loss was **$4.4 \text{ mm}$ of water**[cite: 172].
* [cite_start]**Pump Impact:** This minuscule head loss translates to a pressure drop of **$43 \text{ Pa}$** [cite: 155][cite_start], which is **negligible** ($< 0.002 \%$ of cooling-water pump rating)[cite: 152, 172].

### 3. Mechanical Integrity

* [cite_start]**Hoop Stress:** The calculated hoop stress was $0.6 \text{ MPa}$ for a worst-case design pressure of $0.3 \text{ MPa}$[cite: 135].
* [cite_start]**Safety Factor:** The estimated Safety Factor was **$> 50$** (relative to PLA ultimate tensile strength of $60 \text{ MPa}$)[cite: 135, 142].
* [cite_start]**Burst Test:** The connector successfully withstood a hydrostatic burst pressure of **$0.45 \text{ MPa}$**[cite: 136, 173].

### 4. Chemical Compatibility

| Medium | Observation | Conclusion |
| :--- | :--- | :--- |
| Distilled water ($25 \text{ °C}$) | [cite_start]No change [cite: 138] | [cite_start]**Suitable** for neutral aqueous streams[cite: 139]. |
| $20 \%$ Ethanol | [cite_start]Slight surface whitening [cite: 138] | [cite_start]**Limited Suitability** for solvents[cite: 139]. |
| $2 \text{ M HCl}$ | [cite_start]Surface crazing after $3 \text{ h}$ [cite: 138] | [cite_start]**Not Suitable** for strong acids[cite: 45, 139]. |

## [cite_start]🚀 Design Improvements and Scale-Up [cite: 168, 169]

To extend the utility of the connector for industrial or more demanding lab environments:

1.  [cite_start]**Material Shift:** Upgrade to **PETG** or **Polypropylene (PP)** for better chemical resistance and a higher glass transition temperature ($80 \text{ °C}$ for PETG)[cite: 45, 139, 169].
2.  [cite_start]**Pressure Rating:** Integrate a $1.5 \text{ mm}$ **O-Ring Groove** to embed an elastomer seal, potentially raising the pressure rating to $0.6 \text{ MPa}$[cite: 169].
3.  [cite_start]**Connectivity:** Implement **ISO 7/1 BSP threads** for compatibility with standard metal piping systems[cite: 168].

## Repository Guide

| File/Folder | Content Description |
| :--- | :--- |
| `README.md` | This project overview and summary of findings. |
| `documentation/` | Full **Mini Project Report** PDF. |
| `cad/` | Includes the original CAD file and the **STL** file for direct printing. |
| `printing_files/` | Configuration file detailing the optimized **FDM settings**. |

---

## 2. `cad/Conduit_Connector_STL.stl` (Placeholder)

**Action:** Upload your actual **`Conduit_Connector_STL.stl`** file here. This is the 3D printable object.

## 3. `printing_files/FDM_PLA_Optimized_Settings.txt`

You can use a simple text file to document the exact settings used for the successful prints.

```txt
# FDM Optimized Slicing Parameters for PLA Connector
# Software: Ultimaker Cura (or equivalent)
# Reference: Project Report (Table 3.2)

[Machine & Material]
[cite_start]Material: Polylactic Acid (PLA), 1.75 mm diameter [cite: 117]
Nozzle Diameter: 0.4 mm (Assumed standard)
[cite_start]Nozzle Temperature: 200 C [cite: 117]
[cite_start]Bed Temperature: 60 C [cite: 117]

[Quality]
[cite_start]Layer Height: 0.2 mm [cite: 117]

[Shell]
[cite_start]Wall Thickness: 1.2 mm (Typically 3 perimeters for 0.4mm nozzle) [cite: 117, 165]

[Infill]
[cite_start]Infill Density: 25% [cite: 117]
[cite_start]Infill Pattern: Grid [cite: 117]

[Speed]
[cite_start]Print Speed: 50 mm/s [cite: 117]

[Support]
[cite_start]Support Structure: Removed carefully after printing [cite: 120]

[Post-Processing]
[cite_start]Sanding: Used 400-grit sandpaper for smoothness and tolerance matching [cite: 43, 121]
MIT License

###Copyright (c) [2025] Oviya P

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
