# &GEN SYSTEM

&GEN is a unified, mobile-first bio-computational platform designed to bridge macroscopic biological observation with micro-scale molecular modeling. It integrates field bio-detection, genomic variant mapping, and structure-based drug discovery into an end-to-end digital suite.

---

## Key Features

### 1. &GEN Biological Intelligence (Bio Analyzer)

A multi-modal computer vision and bio-surveillance engine built for real-time field identification.

* **Multi-Class Biological Segmentation:** Detects species, cell types, tissues, organs, and organelles with confidence scoring (e.g., *Scolopendra subspinipes*, *Iris germanica*).


* **SENTINEL Hazard & Biochemical Flags:** Automatically identifies active toxins (e.g., Ssm Spooky Toxin, Phospholipase A2) and issues safety/envenomation protocols.


* **Genomic & Evolutionary Profiling:** Maps observations to gene markers ($COI$, $16S\text{ rRNA}$) and historical lineage classifications.



### 2. &GEN Genomic Mapper (Variant Impact Explorer)

A translational engine for evaluating genetic mutations and their structural consequences.

* **Multi-Database Variant Scoring:** Integrates pathogenicity metrics (AlphaMissense: 0.984, CADD Phred: 34.0, REVEL: 0.942) for mutations such as `TP53 c.818G>A` (`p.Arg273His`).


* **Transcription Factor & Splice-Site Analysis:** Quantifies promoter binding loss ($\Delta\text{Affinity}: -12.7\text{ bits}$) and evaluates splicing disruptions via SpliceAI.


* **3D Structural Stability:** Renders atomic 3D protein structures (PDB: 1TUP) to calculate folding energy changes ($\Delta\Delta G = -2.85\text{ kcal/mol}$), lost hydrogen bonds, and solvent exposure.



### 3. &GEN DRUG (Structure-Based Virtual Screening)

A computational chemistry tool for rational ligand design and binding kinetics.

* **Target-Ligand Docking:** Simulates interactions between target receptors (e.g., HIV-1 Protease, PDB: 1HSG) and small molecules via SMILES input.


* **Affinity & Kinetic Scoring:** Calculates free binding energy ($\Delta G = -11.96\text{ kcal/mol}$) and predicts binding constants ($K_d: 1.71\text{ nM}$, $K_i: 1.85\text{ nM}$, $\text{IC}_{50}: 3.7\text{ nM}$).


* **Pharmacokinetics & ADME:** Evaluates Lipinski's Rule of 5 compliance, ligand efficiency metrics, and active-site hydrogen-bond networks.



---

## Tech Stack

* **Frontend:** Next.js / React, Tailwind CSS, Framer Motion
* **3D Visualization:** 3Dmol.js, Three.js
* **Bioinformatics & Docking Engine:** AutoDock Vina, SpliceAI, Open Babel, PyMOL integrations
* **Machine Learning / Vision:** Custom vision segmentation models, AlphaMissense

---

## Architecture Overview

```
[ Field Image / Input ] ---> [ Biological Intelligence ] ---> [ Species & Toxin ID ]
                                                                     |
[ 3D Structure / PDB ]  <--- [ Genomic Mapper ]          <--- [ Target Gene ]
         |
         v
[ &GEN DRUG Engine ]   ---> [ Virtual Screening ]       ---> [ Affinity & $K_d$ Results ]

```

---

## Getting Started

### Prerequisites

* Node.js 18.0 or higher
* npm or pnpm

### Installation

1. Clone the repository:
```bash
git clone https://github.com/shadmanshakib/andgen-system.git
cd andgen-system

```


2. Install dependencies:
```bash
npm install

```


3. Run the development server:
```bash
npm run dev

```


4. Open `http://localhost:3000` in your browser.

---

## Contact

* **Developer:** Shadman Shakib


* **Email:** shadman.shakib1@g.bracu.ac.bd | shadman.shakiblxl@gmail.com
* **Phone:** +880-1580661064

---

## License & Credits

Build, Design, and Develop: **SHADMAN SHAKIB**

Copyright **SHADMAN SHAKIB**
