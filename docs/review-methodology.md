# Review methodology and corpus

## Search scope

The paper reports searches across Scopus, Web of Science, IEEE Xplore, ScienceDirect, and SpringerLink for work published from 2018 through 2026.

The query family combines terms for:

- financial NLP and financial natural language processing;
- FinBERT, AraBERT, transformers, and LLMs in finance;
- financial sentiment, report summarization, and document classification;
- ESG text analysis and financial information extraction;
- bilingual reporting and Arabic financial NLP.

## Eligibility

Included work addresses NLP or deep learning applied to financial, economic, or ESG text and contributes evidence about model performance, interpretability, or multilingual/bilingual use.

The review excludes purely numerical forecasting, redundant papers, and papers lacking methodological or empirical depth. Hybrid text–numeric work is included when text is a primary modeling signal or when text extraction is a core component.

## Selection process

The prose describes three main selection steps:

1. title and abstract screening;
2. full-text screening;
3. relevance selection supported by backward and forward citation tracking.

Figure 4 instead places citation tracking at the identification stage. Reading the numerical flow consistently gives:

- **1,110 records identified:** 1,024 from database searching plus 86 from citation tracking and reference lists;
- **224 duplicates removed (derived):** 886 records remained for title/abstract screening;
- **540 excluded** at title/abstract screening;
- **346 full texts assessed**;
- **115 full texts excluded:** 42 out of scope, 27 numerical studies, 22 not FNLP studies, and 24 with insufficient methodology;
- **231 studies included**.

Figure 4 itself labels `886` as “Duplicate records removed.” That label conflicts with the next box, which also reports 886 records screened, and with the arithmetic above. This companion treats 886 as the post-deduplication count and 224 as the implied duplicates removed. See [`data/search_flow_counts.csv`](../data/search_flow_counts.csv).

The difference in citation-tracking order is preserved as a presentation inconsistency: the prose calls it the third selection step, while Figure 4 shows it during identification.

## Corpus profile

### Publication year

| Year | Studies | Share |
|---:|---:|---:|
| 2018 | 7 | 3.0% |
| 2019 | 9 | 3.9% |
| 2020 | 20 | 8.7% |
| 2021 | 27 | 11.7% |
| 2022 | 38 | 16.5% |
| 2023 | 47 | 20.3% |
| 2024 | 58 | 25.1% |
| 2025 | 19 | 8.2% |
| 2026 | 6 | 2.6% |

### Method type

| Method family | Studies | Share |
|---|---:|---:|
| Traditional ML | 46 | 19.9% |
| Deep learning | 30 | 13.0% |
| Transformer-based models | 93 | 40.3% |
| LLM-based methods | 39 | 16.9% |
| Hybrid / Document AI | 23 | 9.9% |

### Application domain

| Application | Studies | Share |
|---|---:|---:|
| Financial sentiment and opinion mining | 52 | 22.5% |
| ESG and sustainability analytics | 43 | 18.6% |
| Information extraction from reports | 35 | 15.2% |
| Financial document understanding | 30 | 13.0% |
| Risk, distress, and bankruptcy analysis | 27 | 11.7% |
| Fraud and manipulation detection | 22 | 9.5% |
| Summarization of financial narratives | 16 | 6.9% |
| Question answering and reasoning | 6 | 2.6% |

Machine-readable versions are in [`data/review_counts_by_year.csv`](../data/review_counts_by_year.csv), [`data/review_counts_by_method.csv`](../data/review_counts_by_method.csv), and [`data/review_counts_by_application.csv`](../data/review_counts_by_application.csv).

## Interpretation cautions

- The CSVs are aggregate transcriptions, not the underlying screening database.
- Category totals describe the paper's review design; they should not be treated as a universal census of FNLP.

