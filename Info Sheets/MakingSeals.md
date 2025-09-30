# Guide to O-Rings, Gaskets, and Other Seals

**Context:**  
This document provides guidance on how to implement O-rings and other sealing solutions (such as gaskets, lip seals, 
and face seals) into Unmanned Surface Vehicle (USV) designs.

[Link to Parker O-Ring Manual (ORD-5700)](https://www.parker.com/content/dam/Parker-com/Literature/O-Ring-Division-Literature/ORD-5700.pdf) <br>
[Link to Gask-O-Seal® and Integral Seal™ Design Handbook](https://www.parker.com/content/dam/Parker-com/Literature/Seal-Group/CSS-5124.pdf)

---

## Purpose Statement

The purpose of this guide is to assist USV designers, engineers, and systems integrators in selecting, specifying, and 
applying sealing components—especially O-rings, gaskets, and related seals—to ensure water-tight, pressure-tight, 
corrosion-resistant, and durable interfaces. The document provides best practices, material considerations, 
installation techniques, common failure modes, and design tips to enhance seal performance, reliability, and 
maintainability in marine environments.

---

## Contents

1. Types of Seals: O-Rings, Gaskets, Lip Seals, Face Seals
2. Materials and Compatibility (chemical, thermal, pressure)
3. Seal Profiles, Sizes, and Standards
4. Installation Guidelines and Hardware Interfaces
5. Failure Modes and Diagnostics
6. Design Best Practices for USVs
7. Maintenance, Inspection, and Replacement Strategies
8. References and Further Reading

---

## 1. Types of Seals

**O-Rings:** Circular elastomeric seals widely used for static and dynamic applications. In USVs, they are commonly 
applied in sensor housings, electronic enclosures, and shaft seals.

**Gaskets:** Flat seals, often cut from sheet material, used between flanges or mating surfaces. Useful for large 
access panels, structural joints, and where bolt preload is uneven.

**Lip Seals:** Also known as radial shaft seals, designed to seal rotating or reciprocating shafts. Applied in 
propulsion systems or rotary joints on USVs.

**Face Seals:** Seals compressed between flat surfaces (end caps, hatches, bulkheads). O-rings in face seal glands fall 
into this category.

**Trade-Offs Between O-Rings and Gaskets:** O-rings provide compact, high-pressure sealing and energize under load, 
making them ideal for critical, pressure-tight applications such as AUV hull access panels. However, they require 
precise machining, smooth surface finishes, and uniform bolt preload. Gaskets, while less efficient at holding high 
pressures, are more forgiving to uneven preload and surface irregularities, which makes them useful for large flanges, 
access covers, or structures where machining and torque control are less exacting.
---

## 2. Materials and Compatibility

**Elastomers:**
- **NBR (Nitrile):** Good oil/fuel resistance; limited seawater and UV resistance.
- **EPDM:** Excellent seawater and UV resistance; not recommended for petroleum oils.
- **FKM (Viton):** High chemical resistance, wide temperature range, but more costly.
- **Silicone:** Excellent thermal range; poor abrasion resistance.

**Plastics & Composites:**
- **PTFE:** Excellent chemical resistance, low friction, but limited elasticity.
- **UHMWPE:** High wear resistance; good in sliding gasket applications.

**Metals:**
- **Soft copper or aluminum gaskets:** Used in high-pressure fittings.

**Compatibility Considerations:**
- **Seawater:** EPDM and FKM perform best.
- **Fuel/Oil exposure:** Use NBR or FKM.
- **High Temperature (>150 °C):** Prefer FKM or silicone.

---

## 3. Seal Profiles, Sizes, and Standards

### O-Ring Face Seal Standard

The Parker standard face seal gland (Design Chart 4-3) defines recommended groove dimensions, squeeze values, and radii 
for O-ring face seals. These are widely used in marine and aerospace designs to ensure reliable sealing under static 
face loading.

**Typical Applications in USVs:**
- Sensor housing windows
- Electronics pressure hull end-caps
- Access covers and removable hatches

<img src="Images/MakingSeals/Parking Face Seal Glands.png" alt="Face Seal Glands" width="600" style="border:1px solid #ccc;">

**Simplified Cross-Section Reference (common USV sizes):**

| Cross Section Nominal | Gland Depth (in) | Typical Squeeze % | Groove Width for Liquids (in) |
|------------------------|------------------|------------------|-------------------------------|
| 1/16 (0.070")          | 0.054            | 23%              | 0.107                         |
| 1/8 (0.139")           | 0.101            | 20–30%           | 0.177                         |
| 3/16 (0.210")          | 0.152            | 21%              | 0.270                         |

> **Design Note:** Always break corners with ~0.005" radius, ensure smooth surface finish (≤32 µin for liquids), and apply light lubricant before installation to avoid abrasion. Incorrect gland dimensions or rough surfaces can cause premature O-ring extrusion, compression set, or tearing.

*For complete dimension charts and tolerance specifications, see the [Parker O-Ring Manual (ORD-5700)](https://www.parker.com/content/dam/Parker-com/Literature/O-Ring-Division-Literature/ORD-5700.pdf).*

---

## 4. Installation Guidelines and Hardware Interfaces

- **Surface Finish:** ≤32 µin Ra for liquid seals, ≤63 µin Ra for gas.
- **Groove Design:** Ensure correct gland depth and width for specified squeeze.
- **Compression:** Target 20–30% squeeze on elastomers.
- **Lubrication:** Use silicone grease or Parker O-lube to reduce installation damage.
- **Torquing:** Apply even torque on bolts to avoid uneven squeeze.
- **Alignment:** Ensure concentric alignment of flanges before final tightening.

---

## 5. Failure Modes and Diagnostics

**Common Issues:**
- **Extrusion:** O-ring material forced into clearance gaps under pressure; mitigated with backup rings.
- **Abrasion:** Caused by dynamic surfaces or poor [lubrication](https://bluerobotics.com/store/watertight-enclosures/enclosure-tools-supplies/molykote/).
- **Chemical Attack:** Swelling, cracking, or softening from incompatible fluids.
- **Compression Set:** Permanent deformation after long-term compression.
- **Thermal Aging:** Cracking and hardening from prolonged heat exposure.
- **Swelling:** Caused by fluid absorption.

**Diagnostics:**
- Inspect seals for flattening, cracks, or glossy surfaces.
- Check grooves for sharp edges or contamination.
- Replace seals at the first sign of deterioration.

---

## 6. Design Best Practices for USVs

- **Material Selection:** Choose elastomers with proven seawater and UV resistance (**EPDM**, FKM).
- **Galvanic Isolation:** Electrically isolate stainless fasteners from aluminum housings to reduce galvanic corrosion.
- **Redundancy:** Where failure is critical, use double O-ring barriers.
- **Pressure Variation:** Use [venting](https://bluerobotics.com/learn/pressure-relief-valve-installation-and-usage/) or compensators to avoid pressure differentials.
- **Vibration Resistance:** Avoid designs that rely on adhesive sealing; prefer compression seals.
- **Biofouling Resistance:** Use antifouling coatings around seal areas to prevent marine growth interference.

---

## 7. Maintenance, Inspection, and Replacement Strategies

- **Inspection Intervals:** Every 6–12 months depending on usage and exposure.
- **Signs of Degradation:** Flattening, cracks, brittleness, swelling.
- **Replacement:** Always replace seals during major disassembly; never reuse old O-rings.
- **Spare Parts Management:** Stock common sizes in labeled, climate-controlled storage bags.
- **Field Repairs:** Include spare seals and lubricant in deployment kits.

---

## References and Further Reading

- [Parker O-Ring Manual ORD-5700](https://www.parker.com/content/dam/Parker-com/Literature/O-Ring-Division-Literature/ORD-5700.pdf)

---

### Disclaimer
Markdown formatting and copyediting done with the aid of OpenAI ChatGPT-5. Content was reviewed and curated by  
Tim Mascal, September 2025.

*Prepared by: Embry-Riddle Department of Mechanical Engineering*  
*Last Updated: September 25, 2025*  
