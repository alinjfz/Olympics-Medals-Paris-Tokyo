<div align="center">

# 🥇 Olympic Medals Analysis

### Paris 2024 &nbsp;·&nbsp; Tokyo 2020

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![pandas](https://img.shields.io/badge/pandas-2.0%2B-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/alinjfz/Olympics-Medals-Paris-Tokyo)](https://github.com/alinjfz/Olympics-Medals-Paris-Tokyo)

A comparative data analysis of Olympic medal standings across two consecutive Summer Games — exploring which nations dominated, improved, or declined between Tokyo 2020 and Paris 2024.

</div>

---

## 📋 Overview

<table>
<tr>
<th></th>
<th>🗼 Tokyo 2020</th>
<th>🗼 Paris 2024</th>
</tr>
<tr>
<td><b>Held</b></td>
<td>July – August 2021</td>
<td>July – August 2024</td>
</tr>
<tr>
<td><b>Nations with medals</b></td>
<td>88</td>
<td>90</td>
</tr>
<tr>
<td><b>Total medals awarded</b></td>
<td>~1,080</td>
<td>~1,117</td>
</tr>
</table>

The two datasets are merged on country name, cleaned, and explored through five distinct visualisations.

---

## 📊 Analyses

| #   | Chart                      | Type           | Description                                   |
| --- | -------------------------- | -------------- | --------------------------------------------- |
| 1   | **Combined Medal Count**   | Stacked bar    | Tokyo vs Paris share for top 10 countries     |
| 2   | **Medal Trajectory**       | Horizontal bar | Paris − Tokyo change for all countries        |
| 3   | **Top 5 Risers & Fallers** | Bar            | Biggest movers between the two Games          |
| 4   | **Gold Medal Comparison**  | Grouped bar    | Gold counts side-by-side for top 15 countries |
| 5   | **Global Medal Share**     | Pie chart      | Top 20 nations vs the rest of the world       |

---

## 🗂️ Repository Structure

```
Olympics-Medals-Paris-Tokyo/
├── 📂 data/
│   ├── paris_2024_medals.csv   ← Paris 2024 final medal table
│   └── tokyo_2020_medals.csv   ← Tokyo 2020 final medal table
├── 📓 olympics_medals_analysis.ipynb
├── 📄 requirements.txt
├── 📄 LICENSE
└── 📄 README.md
```

---

## 🚀 Getting Started

### 1 · Clone the repository

```bash
git clone https://github.com/alinjfz/Olympics-Medals-Paris-Tokyo.git
cd Olympics-Medals-Paris-Tokyo
```

### 2 · Install dependencies

```bash
pip install -r requirements.txt
```

### 3 · Launch the notebook

```bash
jupyter notebook olympics_medals_analysis.ipynb
```

> Works in VS Code, JupyterLab, or any Jupyter-compatible environment.

---

## 🔍 Key Findings

> **The United States and China** finished 1st and 2nd in both editions — the only two countries to top 90 combined medals.

- 🇦🇺 **Australia** won 53 medals in Paris, up from 46 in Tokyo — a steady upward trend.
- 🇫🇷 **France** (host nation) surged in Paris with 64 total medals vs 33 in Tokyo.
- 🌍 Several smaller nations — especially in **Central Asia and Africa** — showed the most dramatic upward trajectories.
- 📉 Some historically strong nations saw notable declines, likely reflecting home-advantage effects fading.
- 🌐 The **top 20 countries** claim roughly **75–80%** of all medals across both Games.

---

## 🛠️ Tech Stack

| Tool                                                                                                    | Version | Role                             |
| ------------------------------------------------------------------------------------------------------- | ------- | -------------------------------- |
| ![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat-square)    | 3.8+    | Core language                    |
| ![pandas](https://img.shields.io/badge/-pandas-150458?logo=pandas&logoColor=white&style=flat-square)    | 2.0+    | Data loading, merging, cleaning  |
| ![matplotlib](https://img.shields.io/badge/-matplotlib-11557C?style=flat-square)                        | 3.7+    | Charts and figures               |
| ![seaborn](https://img.shields.io/badge/-seaborn-4C72B0?style=flat-square)                              | 0.12+   | Color palettes and plot styling  |
| ![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?logo=jupyter&logoColor=white&style=flat-square) | 1.0+    | Interactive notebook environment |

---

## 📝 Data Notes

- **Russia (ROC)** — Competed at Tokyo 2020 under the Russian Olympic Committee name due to doping sanctions. Did not compete at Paris 2024. Excluded from trajectory calculations.
- **Name normalisation** — Countries like `"People's Republic of China"` (Tokyo) and `"China"` (Paris) are unified via a mapping dictionary before merging.
- **Missing values** — Countries absent from one dataset are treated as 0 medals for that edition.

---

## 📄 License

Licensed under the [Apache License 2.0](LICENSE) · Copyright 2024 Ali Najafzadeh
