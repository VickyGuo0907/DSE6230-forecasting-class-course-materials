# Forecasting Class — Code & Assignments

Student-facing code repository for **DSE6230: Forecasting Methods and Applications**.
Lecture pages, slides, and the syllabus live in Canvas; the runnable code,
homework, and project guides live here.

## What's in here

| Folder | What it contains |
| --- | --- |
| `notebooks/` | In-class Colab exercises, one per week (`week0N_exercises.ipynb`) |
| `homework/` | Weekly homework assignments as Quarto `.qmd` files |
| `projects/` | Final project guide and the five industry tracks |
| `case_studies/` | Short case studies discussed in lecture (Zillow Offers, Walmart M5, LTCM, …) |
| `class_example/` | A sample syllabus/slides bundle from a prior course as a formatting reference |

## Using the notebooks (Colab)

Each weekly notebook can be opened directly in Google Colab — no local setup
needed. From a notebook in this repo on GitHub, click **Open in Colab**, or
use a URL like:

```
https://colab.research.google.com/github/<your-username>/<this-repo>/blob/main/notebooks/week01_exercises.ipynb
```

## Running locally

If you'd rather run things on your own machine:

```bash
# Python 3.10+ recommended
python -m venv .venv
source .venv/bin/activate           # macOS / Linux
.\.venv\Scripts\Activate.ps1        # Windows PowerShell

pip install pandas numpy matplotlib statsmodels scikit-learn jupyter
jupyter lab
```

The homework `.qmd` files render with [Quarto](https://quarto.org/):

```bash
quarto render homework/homework01.qmd
```

## Homework workflow

1. Open the `.qmd` for that week in your editor (or render it to see the
   instructions).
2. Complete the exercises in a notebook or a copy of the `.qmd`.
3. Submit to Canvas per the assignment instructions.

## Final project

Pick one of the five **Industry Tracks** in [`projects/`](projects/):

- Energy — Grid Load Demand
- Finance — Returns & Risk (M6)
- Supply Chain — Intermittent Demand (M5)
- Retail — Promotion Analysis (Rossmann)
- Economics — Macro-Indicator Forecasting

Full guide: [`projects/README.md`](projects/README.md).

## Primary text

Hyndman & Athanasopoulos, [*Forecasting: Principles and Practice
(Python)*](https://otexts.com/fpppy/). The book is free online; the
companion slides used in lecture are at
[robjhyndman/fpp3_slides](https://github.com/robjhyndman/fpp3_slides).
