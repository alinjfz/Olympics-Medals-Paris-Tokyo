# Olympic Medals Analysis: Paris 2024 vs Tokyo 2020

A data analysis project comparing Olympic medal standings across two consecutive Summer Games.
The goal is to identify which nations dominated, which improved, and how global medal share is distributed.

---

## Overview

| | Tokyo 2020 | Paris 2024 |
|---|---|---|
| Held | July–August 2021 | July–August 2024 |
| Nations with medals | 88 | 90 |
| Total medals awarded | ~1,080 | ~1,117 |

The two datasets are merged on country name, cleaned, and explored through five distinct visualisations.

---

## Analyses

1. **Top 10 countries by combined medals** — stacked bar chart (Tokyo vs Paris share)
2. **Medal trajectory** — horizontal bar chart for all countries (Paris − Tokyo change)
3. **Top 5 risers and fallers** — focused view of the biggest movers
4. **Gold medal comparison** — grouped bar chart for top 15 countries
5. **Global medal share** — pie chart of top 20 countries vs the rest of the world

---

## Repository Structure

```
Olympics-Medals-Paris-Tokyo/
├── data/
│   ├── paris_2024_medals.csv   # Paris 2024 final medal table
│   └── tokyo_2020_medals.csv   # Tokyo 2020 final medal table
├── olympics_medals_analysis.ipynb
├── requirements.txt
├── LICENSE
└── README.md
```

---

## Getting Started

### Prerequisites

Python 3.8 or higher is required. Install dependencies with:

```bash
pip install -r requirements.txt
```

### Run the notebook

```bash
jupyter notebook olympics_medals_analysis.ipynb
```

Or open it in VS Code, JupyterLab, or any compatible environment.

---

## Data Notes

- **Russia (ROC)**: Competed at Tokyo 2020 as the Russian Olympic Committee due to doping sanctions.
  Russia did not compete at Paris 2024. Trajectory calculations exclude Russia.
- **Country name normalisation**: Several countries use different official names across the two datasets
  (e.g. "People's Republic of China" vs "China"). A mapping dictionary in the notebook unifies them.
- **Missing values**: Countries that did not participate in one of the Games are treated as 0 medals
  for that edition when calculating combined totals.

---

## Key Findings

- The **United States** and **China** were the top two nations in both editions.
- **Australia**, **France** (host), and **Great Britain** all showed strong performances in Paris 2024.
- Several smaller nations — including those in Central Asia and Africa — showed notable upward trajectories.
- The top 20 countries account for roughly **75–80%** of all medals awarded across both Games.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| pandas | Data loading, cleaning, and merging |
| matplotlib | Charts and visualisations |
| seaborn | Colour palettes and plot styling |
| Jupyter | Interactive notebook environment |

---

## License

Licensed under the [Apache License 2.0](LICENSE).
