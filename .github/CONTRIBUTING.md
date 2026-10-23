# Contributing to MEDFusion

Thank you for helping keep this companion repository accurate and current.

## What to contribute

- New MMIF methods, datasets, tools or benchmarks published after the survey cutoff.
- Corrections to bibliographic records (DOI, venue, year, author order).
- Fixes for broken links or changed repository names.
- Clarifications to the per-study extraction (`studies_metric_coding.csv`).

## Entry format

Follow the record template used throughout the repository.

For a paper:

```markdown
## [Paper title]
- **Publication**: Journal/Conference, Year
- **Authors**: Author list
- **Core contributions**:
  - Contribution 1
  - Contribution 2
- **Modalities**: MRI-CT / MRI-PET / multi-modal
- **Fusion hierarchy**: Data-level / Feature-level / Decision-level
- **Links**:
  - [Paper DOI](https://doi.org/...)
  - [Official code](https://github.com/...)
```

For a dataset or tool:

```markdown
## [Name]
- **Type**: Registration tool / Dataset / Framework
- **Applicable modalities**: CT / MRI / PET / all
- **License**: Apache 2.0 / MIT / commercial (free for academic use)
- **Links**:
  - [Repository or documentation](https://...)
```

## File and directory conventions

- Place the entry in the directory that matches the manuscript section.
- Use lowercase file names with underscores; never leave trailing spaces in file or directory names.
- One entry per `##` heading; keep the field order of the template.

## Pull requests

1. Open an issue describing the addition or correction.
2. Fork the repository and create a branch.
3. Add or edit the entry, keeping the template and ordering.
4. Describe the source of the information (DOI, publisher page, official repository) in the pull request.
5. The maintainer checks the link and the bibliographic record before merging.

## Per-study extraction

Changes to `studies_metric_coding.csv` must keep one row per study and the existing column set (`uses_*` columns are binary). If a study is added, update the total in the README and regenerate the summary counts.
