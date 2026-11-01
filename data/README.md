# Derived review summaries

This directory contains four small CSV files transcribed or normalized from aggregate information reported in the paper:

- `review_counts_by_year.csv`
- `review_counts_by_method.csv`
- `review_counts_by_application.csv`
- `search_flow_counts.csv`

The three distribution files each total 231 studies. Percentages reproduce the values printed in the paper. For example, `23/231` is approximately `9.96%`, but Table 5 prints `9.9%`; retaining the printed value keeps the column total at `100.0%`.

`search_flow_counts.csv` normalizes Figure 4 into an auditable sequence. Figure 4 labels `886` as “Duplicate records removed,” but the subsequent screening count shows that `886` is the number remaining after duplicate removal. Given `1,110` identified records, the implied number of duplicates removed is `224`.

## Provenance and limitations

- Source: the article identified by DOI `10.1007/s13369-026-11157-6`, especially its review-methodology distribution tables.
- These files contain aggregate facts only; they do not reproduce the paper's prose, figures, or publisher layout.
- They should not be used to infer attributes of individual studies.
- Cite the paper when using these counts in scholarship.

