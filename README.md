# Forecasting Class: Code and Assignments

Student-facing code for DSE6230 Forecasting Methods and Applications.

Lectures, slides, case studies, the syllabus, and the final project guide live in Canvas. The runnable
Jupyter notebooks live here.

## What's in here

| Folder | Contents |
| --- | --- |
| `notebooks/` | In-class exercises, one per week (`week0N_exercises.ipynb`) |
| `assignments/` | Weekly assignments, one per week (`week0N_assignment.ipynb`) |

Every notebook is self-contained: the first code cell installs the packages it needs (`!pip install ...`)
and the next cells pull in the raw data (from a public URL or a built-in dataset loader), so a notebook
runs top to bottom with no separate setup step.

## Running the notebooks

### Google Colab (recommended, no local setup)

From a notebook in this repo on GitHub, click "Open in Colab", or use a URL like:

```
https://colab.research.google.com/github/healeycm/dse6230-forecasting-course-materials/blob/main/notebooks/week01_exercises.ipynb
```

### Locally

```bash
# Python 3.10 or newer recommended
python -m venv .venv
source .venv/bin/activate           # macOS or Linux
.\.venv\Scripts\Activate.ps1        # Windows PowerShell

pip install jupyter
jupyter lab
```

Each notebook installs its own remaining dependencies in its first cell, so no separate `requirements.txt`
is needed.

## Assignment workflow

1. Open that week's notebook in `assignments/`.
2. Run the setup cells (install + data load), then complete the exercises.
3. Submit the completed notebook to Canvas per the assignment instructions.

## Primary text

Hyndman and Athanasopoulos, [*Forecasting: Principles and Practice (Python)*](https://otexts.com/fpppy/).
The book is free online. The companion slides used in lecture are at
[robjhyndman/fpp3_slides](https://github.com/robjhyndman/fpp3_slides).
