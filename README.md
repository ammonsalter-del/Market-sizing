# Market Sizing Workshop

An interactive, self-contained educational tool that teaches students and aspiring entrepreneurs how to build credible, evidence-based market sizing analyses. Built as a single-page web application with no external dependencies.

> **Status:** This tool is currently in **DRAFT** and under active development. Data sources and calculations are being validated.

---

## Overview

Market sizing is a foundational skill in entrepreneurship, strategy, and venture capital — yet it is rarely taught in a structured, hands-on way. This tool fills that gap by combining conceptual frameworks, fully worked examples, a critical-evaluation game, a knowledge quiz, and a guided "build your own" workspace — all in one place.

Students learn the **TAM → SAM → SOM** framework through both **top-down** and **bottom-up** approaches, practise spotting questionable claims in a gamified setting, and leave with a defensible market sizing narrative they can use in a pitch or business plan.

---

## Features

### Learn
Introduces the core concepts — Total Addressable Market (TAM), Serviceable Available Market (SAM), and Serviceable Obtainable Market (SOM) — with visual diagrams, plain-language explanations, and a side-by-side comparison of top-down vs bottom-up approaches.

### Evidence Guide
Teaches students how to find, evaluate, and cite data sources. Covers evidence quality tiers (strong / moderate / weak), the critical distinction between evidence and assumptions, and where to find UK public data (ONS, NHS Digital, Companies House, Defra, HESA, and more).

### Three Worked Examples
Each example includes a full top-down walkthrough, a full bottom-up walkthrough, and a comparison tab explaining convergence.

| Example | Type | Domain | Key Teaching Point |
|---|---|---|---|
| **Hospital Diagnostic Device** | B2B | Healthcare / MedTech | Using NHS Digital ERIC data; filtering by bed count; competitor pricing |
| **Tomato Delivery Service** | B2C | Food / Logistics | Geographic narrowing; observable unit economics; assumption sensitivity |
| **Online Tutoring Platform** | B2C Service | EdTech | Survey intention-action gaps; multi-stage conversion funnels; willingness-to-pay pitfalls |

### Dragon's Due Diligence
A dark-themed mini-game in which the student plays a venture investor evaluating entrepreneur pitches. Over 10 rounds, students decide whether each market claim is **credible** or a **porkie** (i.e. dubious). The game draws from a pool of 28 cases (17 porkies, 11 credible), each with detailed post-answer explanations revealing the reasoning. Trains pattern recognition for:
- Intention-action gaps in surveys
- Unrepresentative samples
- Unsourced or inflated figures
- Unrealistic market penetration assumptions

### Quiz
20 multiple-choice questions covering the entire curriculum, with instant feedback, explanations, and a final score with grade. A full review screen lets students revisit every question.

### Build Your Own
A five-step guided workspace that walks students through creating their own market sizing analysis:

1. **Your Product** — Define the product, customer type (B2B / B2C), and target segment
2. **Top-Down** — Enter TAM with sources, apply SAM and SOM filters with evidence
3. **Bottom-Up** — Define unit price (with basis), purchase frequency, and reachable customers
4. **Sense Check** — Benchmark against industry data, competitors, and comparable companies; run sensitivity analysis (conservative / base / optimistic)
5. **Your Story** — Auto-generates a complete market sizing narrative with an evidence quality audit table, ready for export

### Glossary & FAQ
A searchable glossary of 30+ terms and an FAQ section addressing common student questions (e.g. "How much market share should a new entrant claim?", "Do I need to get the number exactly right?").

---

## Getting Started

### Option 1: Open directly
Simply open `market-sizing-tool.html` in any modern web browser. No server, no installation, no internet connection required.

### Option 2: Serve locally
```bash
# If you'd prefer a local server (optional)
python3 -m http.server 8000
# Then visit http://localhost:8000/market-sizing-tool.html
```

---

## Technical Details

| Property | Detail |
|---|---|
| **Technology** | Vanilla HTML + CSS + JavaScript |
| **External dependencies** | None |
| **File count** | 1 (single self-contained `.html` file) |
| **Approximate size** | ~3,200 lines |
| **Frameworks** | None — no jQuery, React, Vue, or build tools |
| **Browser support** | Any modern browser (Chrome, Firefox, Safari, Edge) |
| **Responsive** | Yes — optimised for desktop and mobile (breakpoint at 768px) |
| **Accessibility** | Semantic HTML, sufficient colour contrast, keyboard navigable |
| **Print support** | DRAFT watermarks hidden in print; export-friendly layout |

---

## Repository Contents

```
├── README.md                        ← This file
├── market-sizing-tool.html          ← The application (open in browser)
└── Market_sizing_example.xlsx       ← Supporting spreadsheet with example data
```

---

## Pedagogical Design

The tool is structured around a **progression of cognitive demand**:

1. **Learn** → _Remember & Understand_ — Absorb the framework and key terms
2. **Evidence** → _Understand & Apply_ — Learn what good evidence looks like
3. **Walkthroughs** → _Apply & Analyse_ — Follow a complete, real-world analysis step by step
4. **Quiz** → _Remember & Evaluate_ — Test recall and judgement
5. **Dragon's Due Diligence** → _Evaluate_ — Critically assess others' claims
6. **Build Your Own** → _Create_ — Produce an original, defensible market sizing

Estimated completion time: **60–90 minutes** for all sections, or modules can be used independently.

### Key Principles Taught
- **TAM → SAM → SOM** as a narrowing framework, not just three numbers
- **Top-down and bottom-up** as complementary lenses — convergence builds credibility
- **Evidence vs assumptions** must be explicitly labelled and tracked
- **Sensitivity analysis** — present ranges, not false precision
- **Source verification** — every number should be traceable to a citable source
- **Demand validation** — the market existing does not mean demand for _your product_ exists

---

## Data Sources Referenced

The tool cites real UK public data sources throughout its examples, including:

- **NHS Digital** — Estates Returns Information Collection (ERIC)
- **ONS** — Office for National Statistics (population, household data)
- **Defra** — Horticulture Statistics, Food Statistics Pocketbook
- **Companies House** — Company registration and financials
- **HESA** — Higher Education Statistics Agency
- **Ofcom** — Annual Monitoring Report on the postal market
- **Sport England** — Active Lives Survey
- **SRA** — Solicitors Regulation Authority statistics
- **BPA** — British Parking Association industry data
- **DfE** — Department for Education school census
- **Kantar / Statista** — Consumer market data

All cited figures have been verified against their primary sources as of early 2025.

---

## Authors

- **Rossella Salandra** — University of Bath
- **Ammon Salter** — Warwick Business School

---

## Licence

This work is licensed under [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You are free to:
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material

Under the following terms:
- **Attribution** — You must give appropriate credit
- **NonCommercial** — You may not use the material for commercial purposes
- **ShareAlike** — If you remix or adapt, you must distribute under the same licence

---

## Contributing

This tool is under active development. If you spot a data error, broken interaction, or have a suggestion, please [open an issue](../../issues) or submit a pull request.

When reporting data issues, please include:
- The section and step where the issue appears
- The current (incorrect) value
- The suggested correction with a citable source
