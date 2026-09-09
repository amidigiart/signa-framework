# SIGNA: Semantic Intent Guarantee and Notary Architecture

**A Certification Framework for AI Output Trustworthiness**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Status: Preprint](https://img.shields.io/badge/Status-Preprint-orange.svg)]()

## Overview

SIGNA (Semantic Intent Guarantee and Notary Architecture) is a certification framework that validates AI outputs across six independent dimensions and issues cryptographically anchored certificates attesting to the validation results.

**Core concept:** A traditional notary certifies that a document *exists*. SIGNA certifies that an AI output's *meaning is real* and its *intention is honest*.

## The Six Pillars

| Pillar | Question |
|--------|----------|
| P1: Semantic Fidelity | Does the output mean what it appears to mean? |
| P2: Intent Alignment | Does the output serve the stated purpose? |
| P3: Emotional Safety | Does the output manipulate affective states? |
| P4: Disinformation Resistance | Is the output free from hallucination? |
| P5: Logical Consistency | Is the reasoning internally sound? |
| P6: Contextual Appropriateness | Is the output suitable for its context? |

## Relationship to CAMP

SIGNA is the **certification function** within [CAMP](https://github.com/amidigiart/camp-protocol) (Cognitive Arbitration Mediation Protocol):

- CAMP **arbitrates** which output to select
- CAMP **mediates** knowledge transfer across transitions
- **SIGNA certifies** what the output means and whether it is trustworthy
- CAMP **anchors** the provenance on blockchain

## Certification Pipeline

```
Consumer Request → Agent de Sens (semantic intake)
    → Provider Routing (via CAMP)
    → TVE 6-Pillar Validation
    → Concordance (multi-agent cross-validation)
    → SIGNA Certificate + Tezos Blockchain Anchor
    → Certified Output → Consumer
```

## Certificate Levels

| Level | Score | Action |
|-------|-------|--------|
| SIGNA-Verified | T ≥ 0.85 | Certificate issued, output delivered |
| SIGNA-Cautioned | 0.65 ≤ T < 0.85 | Certificate with warnings |
| SIGNA-Flagged | 0.40 ≤ T < 0.65 | Human review required |
| SIGNA-Rejected | T < 0.40 | Output blocked |

## Reference Implementation

BRIDGRAI implements SIGNA through 13 components (5 engines + 8 agents) across 5 layers:

- **TVE Core** — Six-pillar validation engine (v0.1)
- **AMIDOR** — Anti-confabulation through competitive dual-AI
- **Concordance Agent** — Multi-agent cross-validation
- **Agent de Sens** — Semantic intake gateway
- **Tezos blockchain** — 128 IP assets anchored on mainnet

## Files

- `SIGNA_Framework_Rosca_2026.md` — Full paper (Markdown)
- `SIGNA_Framework_Rosca_2026.pdf` — Full paper (PDF)

## Related Work

- **CAMP Protocol:** [github.com/amidigiart/camp-protocol](https://github.com/amidigiart/camp-protocol)
- **KCE Framework:** [DOI 10.5281/zenodo.22667873](https://doi.org/10.5281/zenodo.22667873)
- **BRIDGRAI Ecosystem:** [bridgrai.com](https://bridgrai.com)

## Author

**Mihai Roșca**
Independent Researcher, BRIDGRAI Ecosystem
Brăila, Romania, EU
ORCID: [0009-0001-1422-6209](https://orcid.org/0009-0001-1422-6209)

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

## Citation

```bibtex
@misc{rosca2026signa,
  title={SIGNA: Semantic Intent Guarantee and Notary Architecture — A Certification Framework for AI Output Trustworthiness},
  author={Roșca, Mihai},
  year={2026},
  howpublished={GitHub, github.com/amidigiart/signa-framework}
}
```
