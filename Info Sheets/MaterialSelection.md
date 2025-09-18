# Material Selection Considerations for Corrosion in Salt Water Environments

---

## Assumptions

- “Salt water environment” means typical seawater (~3.5% NaCl), ambient to warm temperatures, aerated and with possible bio-activity.
- Costs are for raw stock (metals, composites/polymers) as of *September 2025*; dimensions and suppliers influence cost; values are approximate when derived.
- Material property data are from **MatWeb**, **Rolled Alloys**, and other technical datasheets; corrosion types taxonomy follows *Fontana, Corrosion Engineering (3rd ed.)* and *Uhlig & Revie, Corrosion and Corrosion Control*.

---

## Overview

When selecting materials for marine vessel construction, the primary concern is resisting degradation from electrochemical reactions driven by chloride ions, oxygen, and often microorganisms. Key design trade-offs include balancing **corrosion resistance** (especially pitting, crevice, and galvanic corrosion) with **mechanical strength**, **density/weight**, **fabrication/weldability**, and **cost**. Materials with high chromium, molybdenum, nickel, or special coatings/composites tend to resist localized corrosion much better. But high corrosion resistance often comes with higher costs and sometimes fabrication challenges.

Selecting the right material means quantifying corrosion risks (chloride concentration, flow, oxygen, temperature, biofouling) and matching that with material behavior: how it corrodes, how fast, what mechanical failure modes might result, and total life-cycle cost including maintenance.

---

## Common Corrosion-Resistant Materials

Here are 15 materials (metals + non-metals) commonly used in marine vessel construction and related applications, with their relevant properties, cost estimates, and references.

| Material | Key Seawater Corrosion Resistance Notes | Mechanical / Physical Snapshot | Weldability & Fabrication Issues | Cost (USD/kg) | Reference / Datasheet |
|---|---|---|---|---|---|
| **Stainless Steel 316 / 316L** | Good general corrosion resistance; moderate pitting/crevice; less resistant than duplex/super-duplex in harsh chloride; moderate susceptibility to MIC. | Tensile ~ 515-720 MPa; Yield ~205-290 MPa; Density ~ 8.0 g/cm³; Modulus ~200 GPa. | Weldable; weld heat-affected zones (HAZ) can reduce pitting resistance; careful post-weld passivation helps. | ≈ **$6.50/kg** for sheet stock (McMaster-Carr; sample 316 sheet approx) (convert from per sheet price) | MatWeb: 316 Stainless Steel datasheets; McMaster-Carr: 316 Stainless Steel Sheets :contentReference[oaicite:0]{index=0} |
| **Duplex Stainless Steel 2205 (UNS S32205 / S31803)** | Much better pitting/crevice resistance than 316; high PREN; better resistance to stress corrosion cracking in chloride. Excellent in marine systems. | Tensile ~ 620-900 MPa; Yield ~ 448 MPa; Density ~ 7.82 g/cm³; Modulus ~190 GPa. :contentReference[oaicite:1]{index=1} | More challenging to weld than 316; requires control of heat input to preserve duplex microstructure; careful post-weld treatment is beneficial. | ~ **$12‐14/kg** (supplier plate pricing for 2205 duplex; US rolled alloys quotes) | MatWeb: Outokumpu 2205 datasheet; Rolled Alloys 2205 Data Book :contentReference[oaicite:2]{index=2} |
| **Super Duplex Stainless Steel 2507** | Very high pitting resistance, high PREN; nearly immune to many aggressive chloride / temperature combinations; much more corrosion resistance than standard duplex. | Very high strength; density ~ 7.8-8.0 g/cm³; yield & tensile strengths often 2× that of many austenitics. (Exact values depend on supplier) | Fabrication more difficult: demands controlled welding, preheat/post-weld cooling, etc.; thicker sections may be harder to produce. | ~ **$16-20/kg** (specialty supplier pricing) | (Super Duplex datasheets; comparison charts in Rolled Alloys / other duplex compendia) |
| **Aluminum 5083-H116** | Good resistance to general corrosion; moderate in pitting/crevice; susceptible in welds; good performance in moderately warm seawater; high strength-to-weight. | Tensile ~ 317 MPa; Yield ~ 215 MPa; Density ~ 2.66 g/cm³; modulus ~70 GPa. | Weldable; H116 tempers provide better post-weld corrosion resistance than some other tempers; fabrication needs care to avoid galvanic coupling with more noble metals. | ~ **$4.50/kg** (Al 5083 plate stock from US metal suppliers) | MatWeb Al-5083-H116 datasheet |
| **Aluminum 5086-H116** | Very similar to 5083; somewhat lower strength; good marine hull material; somewhat more corrosion-prone in certain localized situations. | Tensile ~ 290-340 MPa; Density ~2.66 g/cm³; Elongation good; modulus ~70 GPa. | Similar to 5083; welds need to be well protected; anodizing or sacrificial coatings help. | ~ **$4.20/kg** |
| **Aluminum 6061-T6** | Lower corrosion resistance in seawater vs marine-grade Al; chloride attack in welds and heat-affected zones; more susceptible to stress corrosion cracking under certain conditions. | Tensile ~ 310-350 MPa; Yield ~275 MPa; density ~2.70 g/cm³. | Good weldability, but HAZ problems; requires sealing / coatings for marine use. | ~ **$4.00/kg** |
| **Marine Steel AH36 (HSLA steel)** | Good general corrosion if painted/coated; poor resistance to localized corrosion; rusting common; requires surface protection. | Tensile ~ 415-550 MPa; Yield ~250-345 MPa; density ~7.85 g/cm³. | Very weldable; lots of experience; but coatings/galvanizing required; high maintenance. | ~ **$1.50-2.50/kg** (steel plate pricing) |
| **Copper-Nickel 90-10 (Cu-Ni 90/10)** | Excellent resistance to seawater, biofouling; good crevice resistance; moderate pitting; good as lining / piping near seawater intakes. | Tensile ~ 275-380 MPa; density ~8.9 g/cm³; fairly ductile. | More expensive; harder to weld; special welding electrodes required; galvanic concerns when mated with more noble metals. | ~ **$14-16/kg** |
| **Copper-Nickel 70-30 (Cu-Ni 70/30)** | Higher strength and erosion resistance; somewhat less corrosion resistance than 90-10 in some flow / crevice conditions, but better in others. | Higher tensile; similar density ~8.9 g/cm³. | Similar issues; more costly; tends to be used in more stressed components, sometimes in tubing. | ~ **$16-18/kg** |
| **Titanium Grade 2** | Near-immune to corrosion in seawater; excellent resistance to many aggressive forms; very high durability. | Tensile ~350-480 MPa; Yield ~275-345 MPa; density ~4.5 g/cm³; high strength-to-weight; modulus ~105-110 GPa. | Hard to weld; special techniques; cost is high; machining more difficult. | ~ **$35-45/kg** |
| **Titanium Grade 5 (Ti-6Al-4V)** | More strength; slightly more susceptible in some extreme galvanic or crevice conditions vs Grade 2; but still very good. | Tensile ~900 MPa; density ~4.43 g/cm³. | More difficult to weld; risk of beta‐phase formation if mishandled; heat control needed. | ~ **$50-60/kg** |
| **Fiberglass Reinforced Polymer (GFRP)** | Non-metallic, so no electrochemical corrosion; no rust; vulnerable to UV, abrasion, possibly biofouling; resin selection is crucial (vinyl ester / epoxy better). | Density ~1.8-2.0 g/cm³; lower stiffness vs metals; tensile strength depends on fiber/resin; lower shear strength in resin matrix. | Lay-up or molded; joins weaker; edges, cut surfaces need sealing; thermal expansion mismatch. | ~ **$12-20/kg** (composite panel stock; cost varies widely with fiber content) |
| **Carbon Fiber Reinforced Polymer (CFRP)** | Similar electrochemical corrosion advantage; but if carbon conducts, galvanic coupling possible; resin must resist marine environment; excellent strength‐to‐weight. | Density ~1.5-1.7 g/cm³; very high tensile strength; high stiffness; low elongation. | More expensive; sensitive to impact, UV; manufacturing cost and repair cost higher. | ~ **$25-40/kg** |
| **Vinyl Ester Composite (glass + vinyl ester resin)** | Better chemical resistance than polyester; fair seawater resistance; less good than epoxy in marine immersion; biofouling / osmotic effects possible. | Density ~1.9-2.1 g/cm³; moderate tensile strength; modulus lower than CFRP. | Mold or laminate fabrication; edge sealing is important; cost moderate. | ~ **$15-25/kg** |
| **Ultra-High Molecular Weight Polyethylene (UHMWPE)** | Excellent corrosion resistance; no metal corrosion; good abrasion resistance; susceptible to UV and creep under load; not load bearing for structure. | Density ~0.93-0.95 g/cm³; low modulus (flexible); moderate strength. | Difficult to bond; machining; protective UV coatings useful. | ~ **$12-18/kg** |
| **Epoxy / Polyurethane Coatings (marine-grade coatings)** | These are surface barriers: protect substrate; degrade under UV/abrasion; require maintenance; good corrosion inhibition when well applied. | Thin film; negligible structural strength; thickness and adhesion matter more. | Surface preparation critical; re‐coating required; quality of application matters greatly. | ~ **$15-30/kg** (resin + pigment + labor / application cost factored somewhat) |

---

## Galvanic Compatibility Tip

When dissimilar materials are used in contact (electrically and in seawater), galvanic corrosion may cause the less noble (anodic) material to corrode rapidly. Good practice:

- Use metals that are close on the galvanic series (e.g. stainless/duplex paired with 90-10 Cu-Ni is better than stainless with aluminium without isolation).
- Electrically isolate dissimilar metals (gaskets, coatings, non-conductive washers).
- Use sacrificial anodes where needed.
- Apply protective coatings or cathodic protection to vulnerable metals.

---

## Types of Corrosion in Marine Environments

Below are key corrosion types relevant to vessels and marine systems. Each has its own mechanisms, risk factors, and mitigation strategies.

### Uniform (General) Corrosion
An overall chemical or electrochemical attack distributed relatively evenly over a surface. Causes loss of section, but predictable. Common in steel if uncoated. Mitigation: coatings, corrosion allowances.

### Galvanic Corrosion
Occurs when two dissimilar metals are electrically connected in seawater; the more anodic metal corrodes. Example: aluminium fasteners with steel structure. Mitigation: isolate, use compatible metals, or sacrificial anodes.

### Pitting Corrosion
Localized penetration forming small pits. Very dangerous because pits can penetrate quickly without much visible precursor. Promoted by chlorides, low oxygen areas. Materials like duplex/super-duplex stainless or special copper-nickel have high resistance.

### Crevice Corrosion
Occurs in shaded or shielded regions (joints, under deposits, between overlapping plates) where stagnation lowers oxygen. Crevices can lead to concentrated attack. Design to avoid crevices, use seals, flushable design.

### Intergranular Corrosion
Attack along grain boundaries often due to improper heat treatment or exposure to sensitizing temperatures. Austenitic stainless steels suffer this if welded without stabilization or post-weld annealing.

### Selective Leaching (e.g. Dezincification / Graphitic Attack)
When one component of an alloy leaches out (e.g. zinc from brass), leaving a weakened, porous structure. Implications for fittings, valves etc. Use “dezincification‐resistant” brasses or avoid in harsh exposure.

### Erosion-Corrosion
Mechanical wear combined with corrosion, from flowing seawater, abrasion by particles, impeller/blade surfaces. Even corrosion-resistant materials may suffer when flow and turbulence are high. Use harder alloys, coatings, design to avoid turbulence.

### Stress Corrosion Cracking (SCC) / Environmentally Assisted Cracking (EAC)
Cracking driven by tensile stresses (residual or applied) in a corrosive environment (e.g. chlorides for stainless steels, some aluminium alloys). Mitigation: reduce stress, choose resistant alloys (duplex, nickel alloys), control welds and heat affected zones.

---

## Glossary

- **PREN**: *Pitting Resistance Equivalent Number*, an empirical number for stainless alloys: PREN = %Cr + 3.3×%Mo + 16×%N (approx). Higher PREN → better pitting/crevice resistance.
- **Yield Strength**: Stress at which material begins to deform plastically (permanent deformation).
- **Ultimate Tensile Strength**: Maximum stress material withstands before failing in tension.
- **Modulus of Elasticity (Young’s Modulus)**: Measure of stiffness; ratio of stress to elastic strain.
- **Heat-Affected Zone (HAZ)**: Area of metal near weld that is not melted but whose microstructure has been altered by heat, often reducing corrosion resistance.
- **Microbiologically Influenced Corrosion (MIC)**: Corrosion modified or accelerated by the presence of microorganisms in seawater.

---

## References

1. Fontana, M. G. *Corrosion Engineering*, 3rd Edition, McGraw-Hill, Chapters **2**, **5** (forms of corrosion etc.).
2. Uhlig, H. and Revie, R. W., *Corrosion and Corrosion Control*, 4th (or latest) Edition, John Wiley & Sons.
3. *MatWeb Material Property Data Sheets*, e.g. for 316, 2205, aluminium alloy grades. :contentReference[oaicite:3]{index=3}
4. Rolled Alloys, *2205 Duplex Stainless Steel Data Book*. :contentReference[oaicite:4]{index=4}
5. Penn Stainless, “Duplex 2205 Stainless Steel Grade Information”. :contentReference[oaicite:5]{index=5}

---

