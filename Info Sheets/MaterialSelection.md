# Material Selection Considerations for Corrosion in Salt Water Environments

---  

## Overview

When selecting materials for marine vessel construction, the primary concern is resisting degradation from electrochemical reactions driven by chloride ions, oxygen, and often microorganisms. Key trade-offs include balancing **corrosion resistance**, **mechanical strength**, **density/weight**, **fabrication/weldability**, and **cost**.

Some materials are chosen for structural strength (steel, aluminium), others for piping and seawater handling (copper-nickel, bronze), others for coatings or seals (epoxy, EPDM). Selecting the right material means balancing resistance, cost, and maintainability.

---  

## Common Corrosion-Resistant Materials

Here are some materials commonly used in marine construction, hardware, and systems.

| Material                                           | Key Seawater Corrosion Resistance Notes                                                                                                                     | Mechanical / Physical Snapshot                                         | Weldability & Fabrication Issues            | Cost (USD/kg)       | Common Uses                                                                | Reference / Datasheet                                                                                                                       |
|----------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|---------------------------------------------|---------------------|----------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| **Aluminum 6061-T6**                               | Widely available, cheap, general-use alloy; poor corrosion in seawater immersion but common in fittings, masts, above-water parts; anodization recommended. | Yield **276 MPa**; Ultimate Tensile ~310-350 MPa; density ~2.70 g/cm³. | Weldable but HAZ prone; coatings essential. | ~ **$4.00/kg**      | Fittings, deck structures, masts, superstructures                          | [ASM MatWeb: Al-6061 datasheet](https://asm.matweb.com/search/specificmaterial.asp?bassnum=ma6061t6)                                        |
| **Aluminum 5083-H116**                             | Marine grade; excellent hull material; good corrosion resistance in seawater.                                                                               | Yield **228 MPa**; Ultimate Tensile 317 MPa; Density 2.66 g/cm³.       | Good weldability; fabrication care needed.  | ~ **$4.50/kg**      | Ship hulls, decks, frames, bulkheads                                       | [ASM MatWeb: Al-5083 datasheet](https://asm.matweb.com/search/specificmaterial.asp?bassnum=ma5083h116)                                      |
| **Aluminum 5086-H116**                             | Similar to 5083, slightly less strength; widely used in marine hulls.                                                                                       | Yield **207 MPa**; Ultimate Tensile 290 MPa; Density 2.66 g/cm³.       | Weldable; anodization/coatings help.        | ~ **$4.20/kg**      | Patrol boats, fishing vessels, workboats                                   | [ASM MatWeb: Al-5086 datasheet](https://asm.matweb.com/search/SpecificMaterial.asp?bassnum=ma5086h116)                                      |
| **Stainless Steel 316 / 316L**                     | Common marine fasteners/hardware; good resistance but susceptible to crevice/pitting.                                                                       | Yield **205 MPa**; Ultimate Tensile 515 MPa; Density 8.0 g/cm³.        | Weldable; post-weld passivation improves.   | ~ **$6.50/kg**      | Bolts, nuts, rails, fittings, piping                                       | [ASM MatWeb: 316 datasheet](https://asm.matweb.com/search/SpecificMaterial.asp?bassnum=mq316q)                                              |
| **Duplex Stainless Steel 2205**                    | Better pitting/crevice resistance than 316; used in shafts, piping.                                                                                         | Yield **448 MPa**; Ultimate Tensile 621 MPa; Density 7.82 g/cm³.       | Welding requires strict heat control.       | ~ **$12-14/kg**     | Propeller shafts, piping, offshore risers                                  | [MatWeb: Carlson 2205 datasheet](https://www.matweb.com/search/datasheet.aspx?MatGUID=086d8b05d09c4963b95253bd278dc4f4)                     |
| **Super Duplex Stainless 2507**                    | Very high resistance; offshore, subsea oil/gas.                                                                                                             | Yield **530 MPa**; Ultimate Tensile 830 MPa; Density 7.80 g/cm³.       | Demands controlled welding.                 | ~ **$16-20/kg**     | Subsea hardware, heat exchangers, high-stress shafts                       | [MatWeb: Outokumpu SAF 2507® Duplex Stainless Steel](https://www.matweb.com/search/DataSheet.aspx?MatGUID=9d24d6e734b940398ba8409d8fd52aab) |
| **Marine Steel AH36**                              | Very common in ship hulls; corrodes quickly if uncoated; coatings required.                                                                                 | Yield **350 MPa**; Ultimate Tensile 490 MPa; Density 7.80 g/cm³.       | Very weldable; coating/maintenance heavy.   | ~ **$1.50-2.50/kg** | Large ship hulls, bulk carriers, tankers                                   | [MatWeb: ASTM A131 Steel datasheet](https://www.matweb.com/search/datasheet.aspx?matguid=1dcef41729e6420e9612cbd4bec8dc26&n=1)              |
| **Nickel-Aluminium Bronze (NAB)**                  | Excellent seawater resistance, cavitation/erosion resistance; used in propellers, pumps, valves.                                                            | Yield **470 MPa**; Ultimate Tensile 760 MPa; Density 7.58 g/cm³.       | Castable, machinable; harder to weld.       | ~ **$12-18/kg**     | Propellers, seawater valves, pumps                                         | [MatWeb: Nickel Aluminum Bronze datasheet](https://www.matweb.com/search/DataSheet.aspx?MatGUID=cb3c4e0ba6dd4d69a76815c9ccb0c114%0A)        |
| **Copper-Nickel 90-10**                            | Standard for seawater piping and intakes; good biofouling resistance.                                                                                       | Yield **103 MPa**; Ultimate Tensile 276 MPa; Density 8.94 g/cm³.       | Weldable with special electrodes.           | ~ **$14-16/kg**     | Piping, heat exchangers, condenser tubes                                   | [Carlson 90 10 Cu Ni Copper-Nickel Alloy datasheet](https://www.matweb.com/search/datasheet.aspx?matguid=4ef5848662be4c619eb2c87d4667b071)  |
| **Copper-Nickel 70-30**                            | Stronger, erosion-resistant; used in condensers/tubing.                                                                                                     | Yield **88.0 MPa**; Ultimate Tensile 372 MPa; Density 8.94 g/cm³.      | Similar issues; higher cost.                | ~ **$16-18/kg**     | Heat exchangers, desalination tubing                                       | [Copper nickel 30% datasheet](https://www.matweb.com/search/DataSheet.aspx?MatGUID=1de470e1f95c442990e87658c7b6eb36)                        |
| **Titanium Grade 2**                               | Near-immune to seawater corrosion; limited by cost; special military/industrial use.                                                                        | Yield **275 MPa**; Ultimate Tensile 344 MPa; Density 4.51 g/cm³.       | Welds require inert atmosphere.             | ~ **$35-45/kg**     | Heat exchangers, naval hardware, offshore equipment                        | [Titanium Grade 2 datasheet](https://asm.matweb.com/search/specificmaterial.asp?bassnum=mtu020)                                             |
| **Fiberglass Reinforced Polymer (GFRP)**           | Extremely common in small boat hulls; resin choice matters.                                                                                                 | Density ~1.8-2.0 g/cm³.                                                | Easily fabricated; repairs weaker.          | ~ **$12-20/kg**     | Recreational boats, panels, covers                                         | [ISO/ASTM FRP datasheets](https://www.matweb.com/search/datasheet.aspx?matguid=6b8167f8a3f74909b7742e5ed2ff75ec&n=1)                        |
| **Vinyl Ester Composite**                          | Common gelcoat material; good blister resistance.                                                                                                           | Density ~1.9-2.1 g/cm³.                                                | Laminated; needs sealing at edges.          | ~ **$15-25/kg**     | Boat hull coatings, tanks, pipes                                           | Manufacturer datasheets                                                                                                                     |
| **EPDM Rubber (Ethylene Propylene Diene Monomer)** | Outstanding seawater, UV, and weather resistance; widely used in seals, gaskets, flexible couplings.                                                        | Density ~1.1 g/cm³;                                                    | Easy to mold; not structural.               | ~ **$5-7/kg**       | Seals, O-rings, gaskets, hatch covers. [How to make Seals](MakingSeals.md) | ASTM D1418 datasheet                                                                                                                        |
| **Epoxy / Polyurethane Coatings**                  | Essential protective layers for steel and aluminium hulls; periodic maintenance needed.                                                                     | Non-structural film.                                                   | Application quality critical.               | ~ **$15-30/kg**     | Hull coatings, tank linings, protective paints                             | Marine coating standards                                                                                                                    |

---  

## Surface Treatments & Coatings

### Anodization
Aluminium alloys like 6061, 5083, and 5086 benefit from **anodization**, which builds a protective oxide film:
- Increases corrosion resistance.
- Provides better adhesion for paints.
- Improves wear resistance.
- Still vulnerable if mechanically damaged → combine with sealants or paint.

### Other Coatings
- **Epoxy/Polyurethane paints**: Universal for steel hulls.
- **Vinyl ester gelcoats**: Standard for fiberglass hulls.
- **Thermally sprayed aluminium/zinc**: Sacrificial coating for steels.

---  

## Galvanic Compatibility Tip

- Pair metals close on the galvanic series.
- Electrically isolate dissimilar metals.
- Use sacrificial anodes (zinc, aluminium, magnesium).
- Apply protective coatings where needed.

### Galvanic Corrosion Prevention

**Passivated Stainless Steel**
- Stainless steels such as 316 and duplex alloys form a thin, stable oxide film (chromium oxide) when passivated.
- This film reduces the electrochemical potential difference with other materials, lowering the driving force for galvanic corrosion.
- However, the passive layer can break down in chloride-rich environments (like seawater), especially in crevices, leading to localized attack.
- For this reason, relying solely on passivation without design safeguards is risky in marine applications.

**Aluminium vs. Stainless Steel Hardware**
- Aluminium (especially marine alloys like 5083 and 5086) sits far more anodic than stainless steels in the galvanic series.
- When aluminium structures (masts, hull plating, fittings) are joined with stainless steel fasteners, the aluminium will preferentially corrode if there is a conductive seawater path.
- Mitigation strategies include:
    - **Isolators**: Use non-conductive washers, gaskets, or sleeves (e.g., nylon or polymer-coated hardware).
    - **Barrier Coatings**: Apply sealants, anodization, or epoxy coatings on the aluminium surfaces before bolting.
    - **Drainage and Ventilation**: Reduce stagnant seawater at the interface to minimize crevice and galvanic conditions.
    - **Regular Inspection**: Replace or re-coat corroded fastener areas before structural compromise.

In practice, the most effective approach is a combination of **material isolation** and **coatings**, as sacrificial anodes alone often do not sufficiently protect aluminium in direct contact with stainless steel fasteners.


---  

## References

1. [Fontana, M. G. *Corrosion Engineering*, 3rd Edition.](https://erau.primo.exlibrisgroup.com/permalink/01ERAU_INST/15kv1ds/alma99358673405946)
2. [Uhlig & Revie, *Corrosion and Corrosion Control*, 4th Edition.](https://erau.primo.exlibrisgroup.com/permalink/01ERAU_INST/osfi0l/cdi_crossref_primary_10_1023_A_1004112503435)
3. MatWeb Material Property Data Sheets.
4. ASM MatWeb Material Property Data Sheets.

---  

### Disclaimer
Markdown formatting and copyediting done with the aid of OpenAI ChatGPT-5. Content was reviewed and curated by  
Tim Mascal, September 2025.

*Prepared by: Embry-Riddle Department of Mechanical Engineering*  
*Last Updated: September 22, 2025*   
