# Sports Survey Analysis

This project analyzes `response_details.csv` for a sports teammate-finding and court-booking app concept in Ho Chi Minh City.

## Setup

```bash
uv venv .venv
uv pip install --python .venv/bin/python pandas numpy matplotlib nbformat nbclient ipykernel notebook pypandoc-binary
```

## Run the notebook

```bash
.venv/bin/python -m ipykernel install --user --name exe-data-analytic --display-name "Python (exe-data-analytic)"
.venv/bin/jupyter notebook survey_analysis.ipynb
```

Run all cells from top to bottom. The notebook preserves `response_details.csv` and writes derived outputs only.

## Generated outputs

- `data/cleaned_survey.csv`
- `reports/startup_survey_insights.md`
- `reports/survey_methodology_report.md`
- `reports/startup_survey_insights.docx`
- `reports/survey_methodology_report.docx`
- `reports/charts/*.png`
- `reports/tables/*.csv`

## Notes

- `response_details.csv` is treated as anonymized survey data keyed by `UID`.
- The analysis does not load or expose the separate PII/email file.
- The survey was executed via Google Forms, with no incentives offered, and personal identity protected by separating the PII/email data.
