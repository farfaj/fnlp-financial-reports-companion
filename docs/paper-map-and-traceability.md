# Paper map and traceability notes

This guide maps the final 49-page published PDF to its printed journal pages. It is intended to prevent contributors from relying on incorrect internal section references in Table 2 and Section 3.1.

## Final published structure

| Section | Printed page where section begins | Main role |
|---|---:|---|
| 1 Introduction | 11843 | Motivation and scope |
| 2 Research Contributions | 11844 | Contributions and comparison with prior surveys |
| 3 Research Questions | 11845 | RQ1-RQ7 |
| 4 Background Knowledge - Financial Narrative Processing | 11846 | FNP, financial documents, governance, ESG, and Saudi context |
| 5 Search Strategy | 11848 | Search, eligibility, flow, and corpus distributions |
| 6 Review of Existing Studies | 11850 | Method-centered literature synthesis |
| 6.1 Machine Learning and Ensemble Learning Techniques | 11850 | Classical and ensemble methods |
| 6.2 Deep Learning Models and Model Trade-Offs | 11852 | CNN/RNN/LSTM/GRU and trade-offs |
| 6.3 Transformers and Large Language Models | 11856 | Transformer and LLM developments |
| 6.4 Interpretable Models Using Explainable AI (XAI) | 11860 | Explainability literature |
| 7 Comparative Analysis of NLP Tools and Frameworks | 11864 | Extraction and analysis tools |
| 8 Dataset and Sources | 11869 | Dataset/source descriptions |
| 9 Applications | 11875 | Seven application subsections |
| 10 Open Challenges and Future Research Directions | 11877 | Challenges and research directions |
| 11 Explainability and Governance in Financial NLP | 11881 | Governance and deployment considerations |
| 12 Conclusion | 11881 | Conclusions and priorities |

## Corrected research-question routing

Table 2 points RQ1-RQ4 to Sections 4.1-4.4, RQ5 to Section 5, RQ6 to Section 7, and RQ7 to Section 8. Those numbers do not match the final article structure. For navigation, use:

| Research question | Primary final section(s) |
|---|---|
| RQ1 - method evolution | Sections 6.1-6.3 |
| RQ2 - accuracy, interpretability, and scalability trade-offs | Sections 6.2-6.4; Section 11 |
| RQ3 - real-world applications | Section 9 |
| RQ4 - explainability gaps and hybrid/interpretable approaches | Section 6.4; Sections 10.9.3 and 11 |
| RQ5 - tools and platforms | Section 7 |
| RQ6 - multilingual and Arabic-English disclosures | Sections 10.1, 10.4, and especially 10.9.2 |
| RQ7 - transformer/LLM risks | Sections 10 and 11 |

The printed `Section 4.4vInterpretable` entry in Table 2 contains a typographical error. Section 3.1 also describes an earlier section plan that is offset from the final structure.

## Other presentation cautions

- **Search flow:** Figure 4 shows 1,110 identified records and 886 screened records, but labels 886 as duplicates removed. The consistent derived duplicate count is 224. See [Review methodology](review-methodology.md).
- **Citation tracking order:** the prose describes backward/forward citation tracking as the third selection step; Figure 4 places 86 citation-tracking records at identification.
- **Method counts:** Figure 5 has six boxes, its surrounding text says five pillars, and Table 5 counts five categories using a different grouping. See [Method taxonomy](method-taxonomy.md).
- **Dataset numbering:** Section 8 is printed out of order (`8.1`, `8.3`, `8.2`, `8.4` ... `8.9`, `8.9.1`). This companion uses dataset names rather than treating that sequence as a corrected renumbering.
- **Dataset descriptions:** the article's Financial PhraseBank, FinCausal, and CFIE descriptions contain naming or language-label issues. The companion flags these in [Tools and datasets](tools-and-datasets.md) rather than silently repeating them.

## Traceability boundary

The article reports 231 included studies, but it does not publish a 231-row study-level extraction sheet. Its 227 references also include contextual sources, institutional materials, and tool websites. Therefore, neither the reference list nor this companion can support a defensible one-to-one reconstruction of all included-study classifications. The aggregate distributions in this repository remain traceable to Tables 3-5; study-level traceability would require the author's original screening/extraction records or a new independent review.
