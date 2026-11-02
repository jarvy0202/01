# PHARM 610 – Lecture VII: Nano-drug Delivery Systems (Key Points)

Dr. Lavasanifar · Midterm 2 · Based mainly on the lecture transcripts, with the slides as support

---

## 1. Cyclodextrins
- Cyclic glucose oligomers: **α = 6, β = 7, γ = 8** units. Hydrophilic outside, **hydrophobic cavity** inside.
- The drug enters the cavity and forms an **inclusion complex** (1:1 or 1:2) → **solubilizer**.
- **Not useful for targeting: the drug is released too fast.**

---

## 2. Liposomes

**Structure**
- Phospholipid **bilayer vesicles**.
  - Hydrophilic drug → **aqueous core**
  - Hydrophobic drug → **bilayer**
  - Amphiphilic drug → **interface**
- Phospholipids: PC, PE, PS, PI, PG.
  - Fatty acid chains → transition temperature (Tm).
  - Cationic or ionizable head groups → membrane fusion, endosomal escape, RNA loading.
- **Cholesterol → increases rigidity and reduces drug leakage.**

**Preparation**
1. **Thin-film hydration**
   - Lipid in chloroform → rotary evaporation → thin film → hydrate with buffer → large MLVs.
   - **Sonication or extrusion** then makes them smaller and more uniform.
   - This is the old method.
2. **Ethanol injection**
   - Lipid in ethanol, injected into water.
   - Gives smaller, more uniform liposomes; usually no extrusion needed.
3. **Microfluidics**
   - Better mixing; automated and scalable.

- Vesicle types: **SUV, LUV, MLV, MVV** (multivesicular).
- Designs: **conventional, pH-sensitive, cationic, thermo-responsive, immuno- (antibody), stealth/long-circulating (PEG)**.

**Drug loading**
- **Passive:** the drug is added during preparation (organic phase or aqueous phase).
- **Active/remote:** the liposome is formed first, then incubated with the drug.
  - A pH gradient or a salt inside pulls the drug in.
  - **Doxil:** an ammonium sulfate gradient makes doxorubicin **precipitate inside** → very low leakage.

**Quality criteria for generic liposomes (e.g., generic Doxil)**
- Lipid content
- Drug encapsulation
- Size, PDI and charge
- Stability (aggregation, shelf life)
- Drug release

**Other characterization tools**
- **AF4 (field-flow fractionation):** separates particles by size (or charge/density) using flow only, with **no stationary phase**.
- **In vitro release:** dialysis (can be run in USP apparatus 2).
  - Add surfactant or albumin to the release medium to keep **sink conditions** for poorly soluble drugs.

---

## 3. ★ Release Rate → PK → Targeting (core concept)

| Formulation | Drug location | Drug PK |
|---|---|---|
| Rapid release (e.g., Visudyne) | In the bilayer | ≈ **free drug** |
| Sustained release | In the aqueous core | ≈ **carrier** |

- **The slower the release, the more the drug follows the carrier. Slow release is a prerequisite for targeting.**
- Sustained release lowers the effective dose and raises the toxic dose → **higher therapeutic index**.
- Accumulation in tumors and inflamed tissue happens through **EPR**.

---

## 4. ★ Conventional vs Stealth Liposomes

**Conventional (Myocet = doxorubicin; AmBisome = amphotericin B)**
- Opsonins adsorb to the surface → taken up by **MPS / Kupffer cells**.
- Result: **short circulation**, high **liver/spleen uptake**, toxicity with repeated doses.
- AmBisome (1997, SUV, amphiphilic drug at the interface) → **reduced nephrotoxicity**.

**Stealth (PEG)**
- PEG forms a **hydration layer** → blocks protein adsorption → not recognized by MPS → **long circulation**.
- **Stealth + sustained release** → drug is delivered to tumors or inflammation.

---

## 5. ★ Doxil / Caelyx (PEGylated liposomal doxorubicin)

**Formulation**
- About 100 nm; HSPC + cholesterol; **t½ > 50 h**.
- Main benefit: **reduced cardiotoxicity**.

**PK changes compared with free drug**
- ↓ CL
- ↓ Vd
- ↑ t½
- ↑ AUC
- ↑ tumor distribution

**Volume of distribution:** Vd = D_body / C_plasma.
- Free doxorubicin: **254 L**. Doxil: **4.1 L**, about the volume of blood.
- Reason: liposomes are too big to leave normal capillaries, so the drug stays in plasma.

**Why Doxil is still the best formulation:** the precipitated drug barely leaks out.

**Side effects**
- **Decreased:** cardiac and hematologic toxicity, hair loss, neuropathy, vesicant injury, nausea.
- **Increased:** **mucositis** and **hand-foot syndrome (PPE)**.
  - Hand-foot syndrome is thought to come from pressure points squeezing liposomes out of the vessels.
  - Management: **delay the next chemotherapy cycle**.

**Onivyde (liposomal irinotecan, 2015)**
- Irinotecan is a **prodrug of SN-38**. SN-38 is about 1000× more potent but poorly soluble.
- The liposome changes PK the same way Doxil does.

---

## 6. Active Targeting and Triggered Release

**Ligands**
- Antibodies, fragments, nanobodies, aptamers, peptides, folate.
- **Internalizing ligands > non-internalizing ligands.**

**★ Ligand attachment does NOT increase tumor accumulation (EPR still dominates)**
- A high ligand density **masks the PEG stealth layer** → faster clearance.
- Ligands only change the **intratumoral distribution**.

**★ Binding site barrier**
- In **large tumors**, liposomes bind the first cell layer and cannot penetrate deeper.
- Micrometastases and vascular targets are better suited to targeted liposomes.

**★ Post-insertion**
- Ligand-PEG-lipid micelles are incubated with preformed liposomes, and the ligand inserts into the outer leaflet.
- Better than pre-mixing because **more ligand ends up exposed on the surface** (pre-mixing hides some ligand inside).

**ThermoDox**
- A lysolipid liposome designed to release drug at **42 °C**.
- **Failed because it leaked at 37 °C.**

---

## 7. Polymeric Nano/Microparticles

**Materials**
- Natural: gelatin, **albumin**, alginate.
- Synthetic: PLA, PGA, **PLGA**, PCL, PACA.

**Designs**
- **Nanocapsule:** drug core with a polymer shell (reservoir).
- **Nanosphere:** drug dispersed in a polymer matrix.

**Preparation**

| Method | Key point |
|---|---|
| In situ polymerization | Built from **monomers** (emulsion or interfacial); surfactant prevents aggregation |
| Coacervation | Mainly **microparticles / reservoir**; adding a non-solvent makes the polymer coacervate coat the drug core, then it hardens |
| **Emulsion / solvent evaporation** | **Water-immiscible** solvent (chloroform) + PVA; **O/W for hydrophobic drugs, W/O/W for hydrophilic drugs**; used for PLGA |
| **Solvent displacement** | **Water-miscible** solvent (acetone, THF); water is the non-solvent; **smaller particles** |
| Salting out | Like solvent displacement, but an **electrolyte** triggers precipitation |

**Purification (removing free drug)**
- **Dialysis.** Drawback: the drug can migrate to the particle surface, causing **burst release**.
- **Ultrafiltration** (Amicon filters).
- **Ultracentrifugation.**
- **Size-exclusion chromatography (GPC/SEC):** large particles elute first.

**Abraxane (albumin-bound paclitaxel, 2005)**
- Does **not** change PK the way stealth carriers do, but it is clinically effective.

**Steric stabilization**
- A hydrophilic polymer on the surface prevents aggregation.
- It can be **adsorbed** (PVA, Pluronic PEO-PPO-PEO, PEO-PLA) or **chemically grafted** (PEG).

---

## 8. ★ Polymeric Micelles

**Structure**
- Amphiphilic block copolymers above the **CMC** self-assemble into a **core–shell** structure of about **100 nm**.
- **PEG shell** and **hydrophobic core** → solubilize and target poorly soluble drugs.
- Polymers: PEO-b-PPO, PEO-b-PLA, PEO-b-poly(amino acid).

**★ Thermodynamics: the hydrophobic effect (ΔG = ΔH − TΔS)**
- In water, micellization is **endothermic (ΔH > 0)**, so it must be **entropy-driven**.
- Hydrophobic blocks disrupt water's **H-bond network**.
- Hiding them in the core restores that network → **water entropy rises** → ΔG < 0.
- In organic solvents, micellization is **enthalpy-driven**.

**★ Polymeric micelles vs surfactant micelles (Cremophor EL, SDS, polysorbate)**
1. **Lower CMC**, because the hydrophobic block is a macromolecule → they stay assembled after dilution in blood.
2. **Kinetic stability**: a rigid core breaks up over **hours**; liquid-like surfactant cores break up in **milliseconds**.

→ This allows sustained release and targeting after IV injection.

**Drug loading**
- **Dialysis** (DMSO/DMF against water)
- **O/W emulsion** (preformed micelles + drug in chloroform, vigorous mixing, evaporation)
- **Film hydration**
- **Co-solvent evaporation** (acetone, ACN or THF; low boiling point, water-miscible)
- **Microfluidics**

**Clinical examples**

| Product | Drug | Outcome |
|---|---|---|
| NK911 (PEG-poly(Asp)) | Doxorubicin | PK much worse than Doxil → dropped |
| SP1049C (Pluronic) | Doxorubicin (for drug-resistant cancer) | Failed |
| NK105 (PEG-polyaspartate) | Paclitaxel | PK improved (↑AUC, ↑t½) but **missed clinical endpoints** |
| **Genexol-PM (PEG-PDLLA)** | Paclitaxel | **Marketed (Korea, India)**; solubility 5000× water; **no Cremophor EL toxicity** (vs Taxol) |

---

## 9. Likely Short-Answer Questions (with keywords to include)

1. **Why did cyclodextrins fail for targeting?** → Fast drug release.
2. **Where do drugs sit in a liposome? What does cholesterol do?** → Core / bilayer / interface; rigidity, less leakage.
3. **Describe film hydration and how to reduce size.** → Solvent → film → hydrate → MLV → sonicate/extrude.
4. **What is remote loading?** → Preformed liposome + gradient; Doxil ammonium sulfate → precipitation.
5. **Quality criteria for a generic liposome?** → Lipid, encapsulation, size/PDI/charge, stability, release.
6. **Why is slow release needed for targeting?** → Drug PK follows the carrier only if release is slow.
7. **Problems with conventional liposomes?** → MPS uptake, short circulation, liver/spleen toxicity.
8. **How does stealth work?** → PEG hydration layer, no opsonins, long circulation, EPR.
9. **PK changes with Doxil? Why does Vd drop?** → ↓CL, ↓Vd, ↑t½, ↑AUC, ↑tumor; 254 L → 4.1 L because the drug is confined to blood.
10. **Doxil toxicity changes? What is hand-foot syndrome?** → ↓cardiac toxicity; ↑mucositis and HFS (pressure points; delay the cycle).
11. **Does a ligand increase tumor uptake?** → No; it can cost stealth; it changes intratumoral distribution.
12. **Binding site barrier? Post-insertion?** → Large tumors, first cell layer; ligand-PEG-lipid micelles insert into preformed liposomes.
13. **Why did ThermoDox fail?** → Leaked at 37 °C.
14. **O/W vs W/O/W? Emulsion vs solvent displacement?** → Hydrophobic vs hydrophilic drug; immiscible vs miscible solvent (smaller particles).
15. **Purification methods? Drawback of dialysis?** → Dialysis, ultrafiltration, ultracentrifugation, SEC; burst release.
16. **Why is micellization entropy-driven?** → Hydrophobic effect; released water restores its H-bond network.
17. **Polymeric vs surfactant micelles?** → Lower CMC + higher kinetic stability.
18. **Advantage of Genexol-PM?** → Solubilizes paclitaxel without Cremophor EL toxicity.
