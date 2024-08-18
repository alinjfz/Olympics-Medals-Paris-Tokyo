# Olympic Medal Data Visualization

## Overview

This project involves visualizing Olympic medal data from the Tokyo 2020 and Paris 2024 Olympics. The primary goal is to analyze and present the distribution of medals among participating countries, focusing on understanding trends and comparing performance across different games. The project includes various visualizations, such as pie charts and bar charts, to provide insights into medal counts and country trajectories.

## Project Features

- **Data Analysis:** Clean and merge Olympic medal data from Tokyo 2020 and Paris 2024.
- **Visualizations:**
  - Pie chart showing the distribution of medals among the top 20 countries and the "Others" category.
  - Bar charts illustrating the top countries with the most significant upward and downward changes in medal counts.
  - Additional charts and analyses to further explore the data.

## Setup

### Prerequisites

Make sure you have the following Python packages installed:

- `pandas`
- `matplotlib`
- `seaborn`

You can install these packages using pip:

```
pip install pandas matplotlib seaborn
```

## Data Files
This project requires two datasets:

- **df_paris.csv**: Contains medal data for the Paris 2024 Olympics.
- **df_tokyo.csv**: Contains medal data for the Tokyo 2020 Olympics.

Ensure these files are available in the same directory as your Jupyter Notebook or provide the correct path to these files.

## Usage

### Data Preparation:

The datasets are loaded and cleaned to standardize country names and merge data from both Olympics.
Russia is excluded from certain analyses due to data unavailability.
Data Visualization:

A pie chart is created to show the distribution of medals among the top 20 countries and the "Others" category.
Bar charts are used to display the countries with the most significant upward and downward trajectories in medal counts.
Running the Notebook
Open the Jupyter Notebook file (your_notebook.ipynb) and run the cells sequentially to execute the data preparation and visualization steps.

```
jupyter notebook your_notebook.ipynb
```
Replace your_notebook.ipynb with the name of your Jupyter Notebook file.

### Code Explanation
Data Cleaning and Merging
Data Loading: The df_paris and df_tokyo datasets are loaded and processed.
Column Renaming: Column names are standardized for consistency.
Country Name Matching: Country names are unified to handle discrepancies.

### Visualization
**Pie Chart:** Displays the total medal distribution among the top 20 countries and "Others".
Includes both absolute medal counts and percentages.

**Bar Charts:** Show the top countries with the most significant changes in medal counts between Tokyo 2020 and Paris 2024.
Adjustments are made for readability and clarity.
Important Notes
Russia Data Exclusion: Russia's data is omitted from certain visualizations due to sanctions impacting the availability of data.

## Contributions
Feel free to contribute to this project by submitting issues, suggestions, or pull requests. All contributions are welcome!


