# Paper overview

## Publication record

| Field | Final published record |
|---|---|
| Author | Fawaz Khaled Alarfaj |
| Journal | *Arabian Journal for Science and Engineering* |
| Volume and pages | 51:11843–11891 |
| Received | 19 November 2025 |
| Accepted | 3 February 2026 |
| Published online | 28 February 2026 |
| DOI | [10.1007/s13369-026-11157-6](https://doi.org/10.1007/s13369-026-11157-6) |
| Full-text read link | [Springer Nature SharedIt](https://link.springer.com/epdf/10.1007/s13369-026-11157-6?sharing_token=fPcOKmNXc7UOaTEdiK5--_e4RwlQNchNByi7wbcMAY7Hi1hWyzeaoKPAOyZMoMkVcPPZU5svGbGS54KZomjzEByIH4UMJeLFNPhNOycslOJWqeC7myozvWibW0ofr-FkTQPv77BEIkhwN9cUVjbR-OIejJbI1Lv3Jk5z1kAXmcM%3D) |
| Funding reported | King Faisal University, Grant KFU260911 |
| Data availability | The article reports that no datasets were generated or analyzed during the study |

The paper is a review article; its reported 231-study corpus should not be interpreted as a dataset released with the publication.

## Purpose

The review surveys automated extraction and analysis of corporate financial reports and sustainability disclosures using financial natural language processing (FNLP). It connects methodological development with document structure, financial governance, ESG narratives, multilingual reporting, and operational tool choices.

The paper also uses **financial narrative processing (FNP)** as an organizing idea: converting unstructured financial text—annual reports, ESG/CSR disclosures, earnings-call transcripts, and related narratives—into structured, machine-readable information for analysis and decision support.

## Main contributions

The paper contributes:

1. A structured review of shallow machine learning, ensemble learning, deep learning, transformer-based models, and LLM-based approaches.
2. Background on financial document structure and ESG narratives needed to interpret extraction tasks.
3. A comparison of document parsing, OCR, NLP, and financial-analysis tools.
4. A synthesis of applications, limitations, and future research directions.
5. Focused treatment of Arabic–English corporate disclosure in Saudi Arabia and the wider MENA region, linked to Tadawul, ESG reporting, and Saudi Vision 2030.
6. A unifying view that includes layout-aware document understanding, multimodal text–table processing, and explainability rather than treating sentiment classification as the whole of FNLP.

## Research questions

The seven research questions can be read as four connected themes:

| Theme | Questions addressed |
|---|---|
| Method evolution | How FNLP moved from classical ML and deep learning to transformers and LLMs; how accuracy, interpretability, and scalability trade off. |
| Real-world use | How systems support auditing, compliance, ESG reporting, sustainability analysis, and other financial tasks. |
| Tools and multilinguality | Which platforms are useful for report extraction and how Arabic–English disclosures can be aligned reliably. |
| Trust and governance | Where explainability is missing and how hallucination, bias, opacity, and deployment risks should be controlled. |

## Central findings

- FNLP has expanded from short-text classification to long-document, layout-aware, multimodal, temporal, and knowledge-augmented analysis.
- Transformers are the largest method category in the review corpus, but stronger prediction does not remove concerns about auditability, domain shift, latency, cost, or data leakage.
- Document layout, tables, OCR quality, cross-references, and numerical context are first-order modeling problems in financial reports.
- Domain grounding through financial terminology, ontologies, ESG frameworks, and regulatory standards is necessary for dependable use.
- Arabic financial NLP remains under-resourced. Morphology, clitics, specialized terminology, transliteration, and differences between regulatory contexts make naive cross-lingual transfer unreliable.
- Evaluation remains fragmented: many studies use narrow datasets or single splits, and cross-market, cross-domain, cross-lingual, and longitudinal validation are uncommon.
- High-stakes deployment requires explanations that are meaningful to auditors and regulators, source traceability, human review, robustness testing, and governance-aware evaluation.

## How to cite

The companion is a guide to the article, not a replacement for it. Cite the paper using the DOI and consult the published version for authoritative detail.

