# Tools and datasets

## Tool landscape

The paper compares open, research, cloud, SaaS, and proprietary options. These tools are not interchangeable: some recover text, some infer layout and tables, some parse regulatory formats, and others add financial semantics or enterprise search.

| Category | Examples discussed in the paper | Best-fit role | Key caveat |
|---|---|---|---|
| Layout-aware document models | LayoutLM family | Form, table, and visually structured document understanding | Requires document preprocessing and task adaptation |
| Structure and section parsing | FinTOC | Table-of-contents and section extraction | Narrower task and language coverage |
| Regulatory structured data | EDGAR/XBRL tools | Parsing standardized US filings and statement facts | Does not solve arbitrary PDF narratives |
| Cloud document extraction | Amazon Textract; Azure document services | OCR, forms, tables, managed scaling | Usage cost, vendor terms, privacy, and regional availability |
| Open OCR | Tesseract | Baseline OCR across many languages | Quality depends strongly on scans, layout, and preprocessing |
| Commercial OCR/IDP | ABBYY; Docsumo; Parseur | Scanned reports, forms, and template workflows | Licensing and limited transparency |
| Financial search/analytics | AlphaSense; Sentieo; Refinitiv/LSEG tooling | Entity linking, search, filings, calls, ESG | Proprietary data and subscriptions |
| Financial extraction services | Daloopa; ProntoNLP/S&P Global | Structured facts, events, and signals | Enterprise access and opaque models |
| Finance-specific language models | FinBERT variants; BloombergGPT | Sentiment, NER, QA, summarization | Task, access, and compute constraints vary |
| Semantic/graph extraction | Ontology-based tools; financial event extraction systems | Normalized facts and queryable relations | Ontology coverage and maintenance |

The paper's comparison is a research snapshot, not a purchasing recommendation. Product names, capabilities, prices, licenses, and availability can change; verify them with the provider.

## Practical selection questions

1. Is the source born-digital, scanned, image-heavy, or XBRL?
2. Must the system preserve table structure, coordinates, charts, footnotes, and reading order?
3. Which languages and scripts are required, including mixed Arabic–English pages?
4. Is the task extraction, classification, search, summarization, QA, or compliance verification?
5. Can documents leave the organization's environment?
6. Are source citations, confidence scores, and human review mandatory?
7. What licensing, rate, latency, maintenance, and data-residency constraints apply?

## Dataset and source landscape

The review discusses ten commonly used resources or source families:

- **FiQA:** financial opinion mining and question-answering material drawn from news and microblogs.
- **Financial PhraseBank:** sentence-level financial sentiment labels.
- **SEC EDGAR filings:** large-scale US regulatory filings for long-document tasks.
- **Financial Narrative Summarization (FNS):** annual-report narrative summarization.
- **Tadawul ESG reports:** bilingual Arabic–English sustainability and ESG disclosures.
- **Refinitiv ESG corpus:** licensed ESG indicators, narratives, and controversies.
- **Bloomberg financial news:** proprietary financial news used for sentiment and event analysis.
- **FinCausal:** annotated cause–effect relations in financial text.
- **Arabic financial news resources:** Arabic-native financial sentiment and aspect analysis.
- **Corporate financial information extraction corpora:** large narrative resources for extraction and cross-lingual analysis.

## Dataset caveats

- Access ranges from public to licensed and proprietary.
- A public landing page does not imply redistribution rights.
- Small datasets and single train/test splits limit robustness claims.
- EDGAR-scale and commercial corpora can create resource inequities.
- Cross-domain and cross-lingual validation remains uncommon.
- Some dataset descriptions in the paper consolidate related resource families; consult the cited sources before selecting a benchmark.

