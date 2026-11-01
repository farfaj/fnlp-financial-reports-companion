# Method taxonomy

## How the paper's taxonomies relate

The publication uses three views that should not be treated as identical:

- **Figure 5** displays six boxes: Machine Learning, Ensemble Learning, Deep Learning, Transformer Models, Large Language Models, and eXplainable AI.
- The surrounding text calls these the review's “five pillars,” creating a visible count inconsistency with the six boxes.
- **Table 5**, which supplies the 231-study quantitative distribution, uses five mutually exclusive categories: Traditional ML (including SVM/RF/XGBoost and therefore ensemble methods), Deep learning, Transformer-based models, LLM-based methods, and Hybrid/Document AI.

The seven sections below are a **companion synthesis for navigation, not seven mutually exclusive paper categories**. They separate important layers that the paper discusses across sections. Do not attach Table 5 counts directly to these seven sections: ensembles belong inside Traditional ML in Table 5, while Hybrid/Document AI is counted separately there.

## 1. Traditional machine learning

Classical pipelines use lexical counts, TF–IDF, sentiment/readability measures, topic features, named entities, and financial ratios with classifiers such as logistic regression, SVM, random forests, and gradient boosting.

**Strengths:** efficient training, modest data requirements, familiar diagnostics, and competitive performance when features are stable.  
**Limits:** engineered features often miss long-range context, managerial tone, implicit relations, and layout-dependent meaning.

## 2. Ensemble learning

Bagging, boosting, stacking, and dynamic ensemble selection combine models for fraud, distress, bankruptcy, and risk tasks. XGBoost and random-forest families feature prominently in the reviewed work, often with class-imbalance handling.

**Strengths:** robust tabular performance and effective fusion of shallow text with financial variables.  
**Limits:** market- and period-specific features may shift; post-hoc feature importance is not always an audit-grade explanation.

## 3. Deep learning

CNNs capture local textual patterns; RNN, LSTM, and GRU models encode sequence and temporal dependencies. Hybrid architectures combine narrative embeddings with ratios, market signals, or graph structure.

**Strengths:** automatic feature learning and improved use of context.  
**Limits:** labeled-data needs, compute cost, weak cross-market validation, and reduced transparency.

## 4. Transformers and domain adaptation

BERT-family models and finance-adapted variants such as FinBERT improve contextual representation for sentiment, NER, classification, and extraction. AraBERT and multilingual encoders support Arabic and cross-lingual work, but finance-specific adaptation remains limited. Long-document models are relevant because annual reports exceed ordinary context windows.

**Strengths:** strong contextual semantics, transfer learning, and multi-task adaptability.  
**Limits:** domain bias, context truncation, compute requirements, prompt/model sensitivity, and opaque reasoning.

## 5. Layout-aware and multimodal document AI

Models in the LayoutLM family combine token, coordinate, and image information. OCR-free approaches such as Donut operate directly on document images. Table-aware and graph-based systems model row/column structure, hierarchical headings, and relations among cells.

**Strengths:** better fit for visually complex reports, forms, tables, and mixed layouts.  
**Limits:** sensitivity to rotated text, unusual designs, poor scans, spanning cells, reading order, and domain-specific layouts.

## 6. LLMs, retrieval, and knowledge augmentation

LLMs support extraction, summarization, question answering, and reasoning over reports. Retrieval-augmented generation (RAG) grounds responses in indexed passages, while knowledge graphs and ontologies supply domain relations and normalized concepts.

**Strengths:** flexible interfaces, few-shot task adaptation, and richer synthesis.  
**Limits:** hallucination, citation failure, retrieval error, prompt sensitivity, latency, cost, privacy exposure, and limited reproducibility.

## 7. Explainability and hybrid reasoning

The paper covers feature attribution (including SHAP and LIME), attention-based interpretation, graph reasoning, ontology-based extraction, and symbolic–neural combinations. It argues for explanations aligned with financial tasks and regulatory needs, not only generic feature scores.

Promising directions include:

- hierarchical explanations from token to sentence to document;
- counterfactual changes to realistic disclosure language;
- concept-based explanations linked to accounting, ESG, and regulatory taxonomies;
- citation-aware RAG and traceable evidence;
- human-in-the-loop validation and bias audits.

## Cross-cutting evaluation dimensions

> **Companion synthesis, not a finding of the paper.** This table turns evaluation concerns discussed across the review into a practical checklist; it is not reproduced from the article.

Every method family should be assessed across more than predictive accuracy:

| Dimension | Example questions |
|---|---|
| Extraction quality | Are values, units, periods, entities, and table relations preserved? |
| Robustness | Does performance survive OCR noise, layout changes, and linguistic variation? |
| Generalization | Does the system transfer across firms, years, sectors, markets, and languages? |
| Calibration | Are confidence estimates reliable enough for review and escalation? |
| Explainability | Can an auditor trace a decision to evidence and domain concepts? |
| Efficiency | Are latency, compute, maintenance, and licensing costs operationally acceptable? |
| Governance | Are data provenance, privacy, bias, access control, and accountability documented? |

