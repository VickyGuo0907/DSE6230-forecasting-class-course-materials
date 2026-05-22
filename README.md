# Forecasting Class: Code and Assignments

Student-facing code for DSE6230 Forecasting Methods and Applications.

Lecture pages, slides, and the syllabus live in Canvas. The runnable code, homework, and project guides live here.

## What's in here

| Folder | Contents |
| --- | --- |
| `notebooks/` | In-class Colab exercises, one per week (`week0N_exercises.ipynb`) |
| `homework/` | Weekly homework assignments as Quarto `.qmd` files |
| `projects/` | Final-project guide and the five industry tracks |
| `case_studies/` | Short case studies discussed in lecture (Zillow Offers, Walmart M5, LTCM, ...) |

## Using the notebooks (Colab)

Each weekly notebook opens directly in Google Colab with no local setup. From a notebook in this repo on GitHub, click "Open in Colab", or use a URL like:

```
https://colab.research.google.com/github/healeycm/dse6230-forecasting-course-materials/blob/main/notebooks/week01_exercises.ipynb
```

## Running locally

If you'd rather run things on your own machine:

```bash
# Python 3.10 or newer recommended
python -m venv .venv
source .venv/bin/activate           # macOS or Linux
.\.venv\Scripts\Activate.ps1        # Windows PowerShell

pip install pandas numpy matplotlib statsmodels scikit-learn jupyter
jupyter lab
```

The homework `.qmd` files render with [Quarto](https://quarto.org/):

```bash
quarto render homework/homework01.qmd
```

## Homework workflow

1. Open the `.qmd` for that week and read the instructions.
2. Complete the exercises in a notebook or a copy of the `.qmd`.
3. Submit to Canvas per the assignment instructions.

## Final project

Pick one of the five industry tracks in [`projects/`](projects/):

- Energy: grid load demand
- Finance: returns and risk (M6)
- Supply Chain: intermittent demand (M5)
- Retail: promotion analysis (Rossmann)
- Economics: macro-indicator forecasting

Full guide: [`projects/README.md`](projects/README.md).

## Primary text

Hyndman and Athanasopoulos, [*Forecasting: Principles and Practice (Python)*](https://otexts.com/fpppy/). The book is free online. The companion slides used in lecture are at [robjhyndman/fpp3_slides](https://github.com/robjhyndman/fpp3_slides).
