# Asset Comparison Project

**Oregon Quant Group: 5-Week Asset Comparison Project**

**Name:** [FILL IN]
**My pair:** [FILL IN] vs. [FILL IN]
**Core question:** [FILL IN: copy it from the project guide]

This is a starter template: a folder structure plus one notebook per week, with the deliverables laid out.
**You write the code and the analysis.** Replace anything marked `[FILL IN]`.

## What's in here

```
├── README.md                  ← this file
├── requirements.txt           ← the Python packages the project uses
├── data/                      ← downloaded data (never edit these files by hand)
├── figures/                   ← save your charts here for the research note
├── notebooks/
│   ├── 00_setup_check.ipynb   ← START HERE: installs packages and downloads your data
│   ├── week1_returns_and_risk.ipynb
│   ├── week5_data_quality.ipynb
│   ├── week6_volatility.ipynb
│   ├── week7_what_drives_them.ipynb
│   └── week8_systematic_rule.ipynb
└── report/
    ├── research_note_template.md   ← final write-up (~4 pages)
    └── presentation_outline.md     ← final presentation (~5 min)
```

## Getting started

1. Get your own copy of this repo (see [Git basics](#git-basics)).
2. Open the folder in **VS Code** (with the Python and Jupyter extensions) or **JupyterLab**.
3. Open `notebooks/00_setup_check.ipynb` and run the cells from top to bottom.
4. Commit and push.

## Each week

1. Open that week's notebook. Each section is one deliverable from the project guide.
2. Write your code in the empty cells and replace every `[FILL IN]`.
3. Save the charts you'll need for the research note to `figures/`, e.g. `fig.savefig("../figures/week1_returns.png")`.
4. Restart the kernel and **Run All** to make sure everything runs top to bottom.
5. Commit and push.

## Final deliverables (finals week)

1. **Research note (~4 pages):** `report/research_note_template.md`
2. **Code:** clean and commented. A peer should be able to click **Run All** and get your exact charts.
3. **Presentation (~5 minutes):** `report/presentation_outline.md`

## Ground rules

- Never edit the downloaded CSV files by hand. Fix data problems in code.
- Keep your date range fixed so your results don't change when you re-run.
- In backtests, shift your signal by one day: `position = signal.shift(1)`.

## Git basics

Always navigate into your project folder in the terminal first:

```bash
cd path/to/your/project-folder
```

Save and upload your work:

```bash
git add .
git commit -m "Short description of what you did"
git push
```

| Command | What it does |
|---|---|
| `git status` | Shows what has changed |
| `git add .` | Stages everything for the next commit |
| `git commit -m "..."` | Saves a snapshot |
| `git push` | Uploads your commits to GitHub |
| `git pull` | Downloads changes (do this first if you work on two computers) |

## Troubleshooting

| Problem | Fix |
|---|---|
| `pip` isn't recognized in the terminal | Use the install cell in `00_setup_check.ipynb` instead |
| `ModuleNotFoundError` right after installing | Restart the kernel, then run the cell again |
| `FileNotFoundError` for `../data/...` | Run the setup notebook first, and check the ticker spelling in the file name |
