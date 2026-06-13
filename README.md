# TASSH Hypertension Intervention Analysis

This project analyzes data from a pragmatic cluster randomized trial in Ghana evaluating whether health insurance coverage plus a nurse-led task-shifting intervention reduced systolic blood pressure more than health insurance coverage alone.

The analysis was completed for an undergraduate biostatistics and epidemiology course and is organized here as a reproducible statistical portfolio project.

## Research Question

Among adults with newly diagnosed hypertension in Ghana, does assignment to health insurance coverage plus the TASSH nurse-led task-shifting intervention lead to a greater reduction in systolic blood pressure over 12 months compared with health insurance coverage alone?

## Methods

I used a linear mixed-effects model to account for the study design:

- Repeated systolic blood pressure measurements within participants
- Participants clustered within community health centers
- Fixed effects for treatment arm, time, and the treatment-by-time interaction
- Random intercepts for clinic and participant

The primary comparison was the treatment-by-time interaction at 12 months, representing the difference in systolic blood pressure change between the intervention and control groups.

## Files

- `SDS390FinalFloer_eval.qmd`: reproducible Quarto report with R code and narrative
- `SDS390FinalFloer_eval.pdf`: rendered final report
- `data/tassh_analysis_wide.csv`: processed participant-level analysis dataset
- `data/tassh_analysis_long.csv`: processed long-format dataset used for mixed-effects modeling
- `references.bib`: bibliography for the report
- `apa_1.csl`: citation style file used by Quarto

## Skills Demonstrated

- Data cleaning and reshaping with `tidyverse`
- Longitudinal data analysis
- Mixed-effects modeling with `lme4` and `lmerTest`
- Model comparison using likelihood ratio tests
- Missingness assessment
- Reproducible reporting with Quarto

## Data Source

The de-identified trial data used for this analysis are publicly available through Zenodo: <https://zenodo.org/records/4949370>.

The CSV files in `data/` are processed analysis datasets derived from the public source data. Raw downloaded spreadsheet files are not included in this repository.



