# Visualization of COVID-19 Cases in Spain

This repository contains an analysis and visualization of confirmed COVID-19 cases in Spain, specifically focusing on the region of Andalusia. The goal of this project is to explore and visualize the evolution of cases over time using various R-based techniques.

![Alternative text](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41598-023-33795-8/MediaObjects/41598_2023_33795_Fig1_HTML.png)

## Project Overview

- **Objective**: To analyze and visualize the evolution of confirmed COVID-19 cases in Andalusia using data from a provided dataset.
- **Dataset**: The dataset includes various columns such as declaration date, region, confirmed cases (PCR), hospitalizations, ICU admissions, recoveries, and deaths.

## Analysis and Visualizations

1. **Initial Setup**:
   - Load necessary libraries: `readxl`, `dplyr`, and `ggplot2`.
   - Load the dataset using `read_excel` and filter it to focus on Andalusia. The data is also sorted by the declaration date.

2. **Bar Chart Visualization**:
   - A bar chart is created to represent the evolution of confirmed PCR cases in Andalusia over time.
   - The chart uses a gradient color scale from yellow to red to represent the intensity of confirmed cases.

3. **Point Plot Visualization**:
   - A point plot is created to represent the same data, using points instead of bars.
   - The points are colored based on the number of confirmed cases, with a similar gradient from yellow to red.

4. **Line and Area Plot Visualization**:
   - A combined line and area plot is created to show the evolution of confirmed cases.
   - The line is colored with a gradient, and the area under the curve is filled with a semi-transparent color. The maximum number of confirmed cases is highlighted using the `annotate` function.

5. **Comparative Visualization**:
   - A bar chart is created to represent both confirmed PCR cases and ICU admissions over time in Andalusia.
   - The chart uses a different color gradient and a modified theme from the `ggthemes` library.

6. **Weekly Aggregated Data Visualization**:
   - The data is aggregated by week, and a grouped bar chart is created to show the weekly totals for confirmed cases, hospitalizations, ICU admissions, recoveries, and deaths.
   - The `gather` function from `tidyr` is used to reshape the data for visualization.

## Conclusion

The first bar chart is considered the most effective in representing the evolution of confirmed COVID-19 cases due to its clear depiction of attribute sizes and more representative color usage. The analysis also explores the relationship between confirmed cases and ICU admissions, noting anomalies in the data.

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/spain-covid19-visualization.git
   ```
2. **Install dependencies**:
   ```bash
   install.packages(c("readxl", "dplyr", "ggplot2", "ggthemes", "lubridate", "tidyr"))
   ```
3. **Run the R scripts:** Open the R Markdown file to explore the analysis and generate the visualizations.
