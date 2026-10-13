# Unemployment Analysis in India Using Python

## Project Overview

This project explores unemployment trends across India using Exploratory Data Analysis (EDA). The primary objective is to identify regional differences in unemployment rates, analyze changes over time, and investigate the sharp increase in unemployment during the COVID-19 period.

The analysis uses Python-based data manipulation and visualization techniques to extract meaningful insights from historical unemployment data.

## Objectives

- Analyze average unemployment rates across regions.
- Identify regions with the highest average unemployment rates.
- Examine monthly unemployment trends from May 2019 to June 2020.
- Compare unemployment trends across Maharashtra, Haryana, and Bihar.
- Investigate relationships between unemployment, estimated employment, and labour force participation.
- Compare unemployment levels before March 2020 with those during the COVID-19 period.

## Dataset

The dataset contains regional unemployment information with the following columns:

- `Region`: Name of the state or region.
- `Date`: Observation date.
- `Frequency`: Frequency of the observation.
- `Estimated Unemployment Rate (%)`: Estimated unemployment rate.
- `Estimated Employed`: Estimated number of employed people.
- `Estimated Labour Participation Rate (%)`: Estimated labour force participation rate.
- `Area`: Rural or urban classification.

**Dataset coverage:** May 2019 – June 2020.

The notebook removes completely blank rows and converts the date column into datetime format before conducting the analysis.

## Tech Stack

- **Python** — Core programming language
- **Pandas** — Data cleaning, manipulation, and aggregation
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization and heatmaps
- **Jupyter Notebook** — Interactive analysis

## Methodology

1. **Data loading and inspection:** Examined the dataset's structure, dimensions, data types, and missing values.
2. **Data cleaning:** Removed completely empty rows and converted dates into the appropriate format.
3. **Regional analysis:** Calculated average unemployment rates and identified the ten regions with the highest averages.
4. **Time-series analysis:** Examined monthly unemployment trends throughout the dataset's coverage period.
5. **Regional comparison:** Compared unemployment trends across Maharashtra, Haryana, and Bihar.
6. **Correlation analysis:** Used a correlation matrix and heatmap to examine linear relationships between selected numerical variables.
7. **COVID-period comparison:** Compared unemployment levels before March 2020 with those from March 2020 onward.

## Key Findings

- Average unemployment remained around 9–10% from May 2019 through February 2020 in the analyzed dataset.
- The average unemployment rate increased sharply to approximately **23.64% in April 2020** and **24.88% in May 2020**.
- The average rate subsequently declined to approximately **11.90% in June 2020**.
- Tripura and Haryana recorded some of the highest average unemployment rates among the regions analyzed.
- The analysis highlights considerable regional variation and a pronounced increase in unemployment during the early COVID-19 period.

These findings describe patterns in the dataset and do not, by themselves, establish causal relationships.

## Visualizations

The Jupyter Notebook includes:

- Bar chart of the ten regions with the highest average unemployment rates.
- Monthly unemployment trend line chart.
- Time-series comparison of Maharashtra, Haryana, and Bihar.
- Correlation heatmap of unemployment, estimated employment, and labour force participation.

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Grouping and aggregation using Pandas
- Time-series data analysis
- Correlation analysis
- Statistical visualization
- Interpretation and communication of data-driven insights

## Project Structure

```text
DATA SCIENCE -Task 2- Unemployment Analysis with Python/
├── Unemployment_Analysis.ipynb
└── README.md
```

## Limitations

This analysis is based on historical data covering May 2019 to June 2020. The correlation analysis identifies linear associations, not causation. The observed changes during the COVID-19 period should therefore be interpreted as temporal patterns rather than definitive proof of causality.

## Conclusion

This project demonstrates how Python-based exploratory data analysis can be used to investigate regional differences, identify temporal patterns, and communicate insights through visualizations. It strengthened my understanding of data cleaning, aggregation, time-series analysis, and responsible interpretation of statistical relationships.

**Project category:** Data Science | Exploratory Data Analysis

**Author:** Punya Mehta