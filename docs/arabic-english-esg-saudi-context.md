# Arabic–English, ESG, and Saudi context

## Why the regional context matters

The paper treats Saudi Arabia and the wider Gulf/MENA setting as more than a geographic example. Market rules, reporting standards, language choice, disclosure conventions, sector composition, and national strategy all affect how an FNLP system should be designed and evaluated.

Saudi Vision 2030, the Capital Market Authority, and Saudi Exchange (Tadawul) reporting provide the policy and market setting. The review connects automated financial and ESG analysis to transparency, sustainability, regulatory oversight, investor due diligence, and cross-border comparability.

## Bilingual disclosure is not simple translation

Arabic–English reports can differ in layout, segmentation, terminology, and the level of detail disclosed. A dependable pipeline must distinguish genuine semantic inconsistency from ordinary translation or formatting variation.

Key Arabic NLP challenges described in the paper include:

- root-and-pattern morphology;
- attached prefixes, suffixes, and clitics;
- tokenization fragmentation in subword models;
- specialized finance and ESG terminology;
- English transliteration and code-switching;
- right-to-left and mixed-direction layout;
- limited standardized Arabic financial benchmarks;
- regulatory and cultural differences that weaken direct transfer from English models.

## ESG extraction requirements

Financial and sustainability disclosures combine quantitative metrics with narrative commitments. Useful extraction therefore requires:

- value, unit, period, scope, and entity resolution;
- distinction between targets, historical results, and aspirational claims;
- links between narrative text, tables, footnotes, and charts;
- normalization to frameworks such as GRI and SASB where appropriate;
- temporal comparison and contradiction detection;
- evidence for greenwashing review and compliance checks;
- cross-language alignment that preserves regulatory meaning.

## Suggested evaluation design

A Saudi bilingual FNLP benchmark should separate and report:

1. Arabic-only, English-only, and mixed-language performance;
2. native PDF versus OCR-dependent documents;
3. text, table, and text–table consistency tasks;
4. sector, issuer, and reporting-year generalization;
5. literal translation alignment versus concept-level regulatory equivalence;
6. extraction accuracy, calibration, evidence traceability, and reviewer agreement;
7. error profiles for morphology, numerals, currencies, dates, units, and directionality.

## Responsible interpretation

The paper motivates this agenda but does not release a Tadawul benchmark, trained bilingual model, or production compliance system. Claims about readiness for regulatory use require separate empirical validation, legal review, and human oversight.

