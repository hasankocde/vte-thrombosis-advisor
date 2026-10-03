# 🩺 AWMF-S2k Venous Thromboembolism (VTE / DVT / PE) — Clinical Advisor

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Guideline](https://img.shields.io/badge/AWMF--S2k-VTE_&_PE_Guideline-critical.svg)](https://www.awmf.org)
[![Evidence-Based](https://img.shields.io/badge/Clinical_Recommendations-Soll_|_Sollte_|_Kann-green.svg)](https://www.awmf.org)

An **evidence-based clinical AI advisor** for Venous Thromboembolism (VTE), Deep Vein Thrombosis (DVT), and Pulmonary Embolism (PE), powered by the official **AWMF-S2k Guidelines** (226 pages). Built for agentic AI architectures (Google Antigravity, Claude Code, Cursor, and LLM frameworks) with strict **zero-hallucination negative constraints**, page-level citations (`--- [PAGE X] ---`), and verified recommendation grades (`Soll ⇑⇑` / `Sollte ⇑` / `Kann ⇔`).

---

## 🌟 Key Features

- **Official AWMF-S2k Source Knowledge:** Full 226-page clinical guideline text and all 45 structured guideline tables and clinical prediction scores.
- **45 Structured Tables & Clinical Scores:** Wells DVT & PE, revised Geneva score, age-adjusted D-Dimer threshold, sPESI early mortality risk, HESTIA outpatient criteria, Villalta PTS score, Constans UEDVT score, and VTE-BLEED bleeding score.
- **Precision DOAC/NOAC Regimens:** Exact acute loading, maintenance, extended secondary prophylaxis dosing, and renal cut-offs for Apixaban, Rivaroxaban, Edoxaban, and Dabigatran.
- **Emergency Protocols & Specific Antidotes:** Structured management for massive PE, rescue thrombolysis, catheter-directed interventions, and specific DOAC reversal (Idarucizumab, Andexanet alfa, 4F-PCC, Protamine).
- **Special Clinical Scenarios:** Cancer-associated thrombosis (CAT), pregnancy & peripartum anticoagulation, upper extremity DVT, splanchnic/cerebral vein thrombosis, and anticoagulation failure.

---

## 📁 Repository Structure

```text
vte-thrombosis-advisor/
├── SKILL.md                          # Agent instructions, negative constraints, and agentic loop
├── README.md                         # Detailed documentation and usage instructions
├── LICENSE                           # MIT License
└── guidelines/                       # Guideline knowledge base
    ├── TABLES_AND_SCORES.md          # 45 official guideline tables & clinical scores
    ├── TABELLEN_UND_SCORES.md        # German reference table compendium
    └── Venenthrombose-Lungenembolie.txt # Full 226-page guideline text with page & recommendation tags
```

---

## 🚀 Installation & Usage

### 1. In Google Antigravity
Clone or copy this directory into your Antigravity skills path:
```bash
git clone https://github.com/hasankocde/vte-thrombosis-advisor.git ~/.gemini/config/skills/vte-thrombosis-advisor
```

### 2. In Other Agentic Frameworks (Claude Code, Cursor, AutoGen)
Point your agent to `SKILL.md` as the core system/skill instruction, ensuring access to `./guidelines/`.

### Example Clinical Inquiries
> *"A 68-year-old patient with an acute unprovoked proximal DVT has a GFR of 42 ml/min. What are the recommended DOAC regimens according to the AWMF-S2k guideline, including initial and maintenance dosing? Provide exact page citations and recommendation grades."*

> *"What is the emergency reversal protocol for a patient on Apixaban 5 mg BID presenting with life-threatening intracranial hemorrhage?"*

---

## ⚖️ Medical Disclaimer

This skill and its repository are intended for **educational, clinical research, and clinical decision support purposes only**. They do not constitute formal medical practice, diagnosis, or individualized treatment plans. Always consult current official institutional protocols and professional medical judgment.

## 📖 Attribution
Based on the official German **AWMF S2k-Leitlinie: Diagnostik und Therapie der Venenthrombose und Lungenembolie** (AWMF-Registernummer 065-002). Official documents are maintained at [awmf.org](https://www.awmf.org).
