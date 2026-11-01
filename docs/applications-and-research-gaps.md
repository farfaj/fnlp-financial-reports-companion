# Applications and research gaps

## Application areas

Section 9 of the paper presents seven connected decision-support areas:

- **Policy and finance insight:** identify policy-relevant statements, sustainability commitments, and investment themes.
- **Transparency and accountability:** extract facts and detect inconsistencies across narrative, tables, periods, and external standards.
- **Greenwashing analysis:** flag vague language, unsupported claims, and divergence between commitments and reported performance.
- **Strategic planning and forecasting:** track forward-looking statements, themes, risks, and technology adoption over time.
- **ESG benchmarking:** normalize metrics and compare qualitative and quantitative disclosures across companies and sectors.
- **Regulatory compliance monitoring:** identify missing disclosures, anomalies, and deviations from reporting requirements.
- **Investor decision support:** structure entities, relations, risks, and strategies from long reports.

Table 4 separately counts **fraud/manipulation detection**, **summarization of financial narratives**, and **question answering/reasoning** as review-corpus application categories. They are not additional subsections of Section 9.

These applications support review and prioritization. They do not remove the need for professional judgment.

## Open challenges

### Language and context

Financial prose is dense, hedged, domain-specific, and filled with cross-references and forward-looking statements. The same ESG phrase can carry different legal or cultural implications across jurisdictions.

### Document variability

Reports mix columns, tables, images, charts, appendices, footnotes, and decorative layouts. Scanned or degraded PDFs introduce OCR errors that propagate into downstream models.

### Verification and consistency

Models must reconcile narrative and tables, resolve entities and periods, handle rare but consequential inconsistencies, and preserve evidence paths.

### Robustness and generalization

Reported accuracy can hide data leakage, overfitting, distribution shift, and sensitivity to corruptions or prompts. Cross-market, multilingual, and longitudinal tests are needed.

### Evaluation maturity

Accuracy, precision, recall, and F1 are insufficient by themselves. Calibration, robustness, operational latency, compute cost, maintainability, auditability, and human-review outcomes matter in practice.

### Explainability and governance

High-stakes systems need domain-meaningful explanations, bias assessment, human escalation, privacy controls, provenance, and clear accountability. LLMs add hallucination, prompt sensitivity, opaque reasoning, and citation risks.

## Research agenda

The paper supports the following priorities:

1. standardized benchmarks spanning reports, ESG disclosures, languages, layouts, and markets;
2. domain-adaptive pretraining and morphology-aware Arabic processing;
3. joint text–table–image models with consistency checks;
4. cross-market, cross-domain, cross-lingual, and longitudinal validation;
5. explainable-by-design symbolic–neural architectures;
6. task- and regulation-oriented explanations rather than generic feature attribution alone;
7. RAG with citation-aware reasoning;
8. model calibration, sensitivity analysis, and stress testing;
9. human-in-the-loop workflows with auditable evidence;
10. governance frameworks covering privacy, bias, cost, maintenance, and regulatory change.

## A useful deployment gate

> **Companion synthesis, not a finding of the paper.** The four-gate checklist below operationalizes themes discussed across the paper; the paper does not present this exact framework.

Before an FNLP prototype influences a financial, audit, compliance, or ESG decision, require affirmative evidence for all four gates:

| Gate | Minimum evidence |
|---|---|
| Data | lawful access, provenance, representative languages/layouts, leakage controls |
| Model | task accuracy, robustness, calibration, cross-domain tests, documented failure modes |
| Evidence | source traceability, extraction lineage, reproducible outputs, meaningful explanations |
| Operations | human review, access controls, monitoring, change management, accountability |

