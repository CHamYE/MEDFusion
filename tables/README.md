# 📋 Tables from the Manuscript

Every table in the manuscript is reproduced here in Markdown so that the repository can be read and diffed without opening the PDF. Tables 3–5 are also released as CSV.

| Table | File | Rows | Also available as |
|---|---|---|---|
| 1. Comparison with prior surveys | [table1_comparison.md](table1_comparison.md) | 13 | — |
| 2. Configurations across the three axes | [table2_mapping.md](table2_mapping.md) | 6 | — |
| 3. Data-level fusion studies | [table3_data_level.md](table3_data_level.md) | 48 | [CSV](table3_data_level.csv) |
| 4. Feature-level fusion studies | [table4_feature_level.md](table4_feature_level.md) | 153 | [CSV](table4_feature_level.csv) |
| 5. Decision-level fusion studies | [table5_decision_level.md](table5_decision_level.md) | 10 | [CSV](table5_decision_level.csv) |
| 6. Cross-generation comparison | [table6_cross_generation.md](table6_cross_generation.md) | 8 | — |
| 7. Reported quantitative results (GLIS-RT) | [table7_reported_quantitative.md](table7_reported_quantitative.md) | 16 | — |
| 8. Software components and records | [table8_tools.md](table8_tools.md) | 17 | — |
| 9. Public datasets | [table9_datasets.md](table9_datasets.md) | 10 | — |
| 10. Evaluation system | [table10_evaluation.md](table10_evaluation.md) | 7 | — |

## 🗒️ Notes on the conversion

- Tables 3–5 list **211 entries** from **192 distinct studies**; a study that appears in more than one configuration is repeated, as in the manuscript. The per-study extraction (one row per study) is in [`studies_metric_coding.csv`](../studies_metric_coding.csv).
- Citation markers were converted to DOI links using `refs_R1.bib`; the paper title itself is the link. Where a record has no DOI, the title is left unlinked (9 rows in Table 3, 21 in Table 4, 2 in Table 5).
- Mathematical notation is written in plain text (`Q^AB/F`, `e_max`). The typeset formulas remain in the manuscript PDF.
- Tool names in Table 8 link to their official sites; dataset names in Table 9 link to the source portal.
- Table 10 keeps the two-level structure (dimension, then measure); formula rows are represented by the measure name only.
