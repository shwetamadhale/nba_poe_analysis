# NBA Shot Logs Analysis and Clustering

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Implementation Steps](#implementation-steps)
- [Example Code](#example-code)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## Overview
This project analyzes NBA shot log data to identify factors affecting shooting efficiency and applies clustering techniques to group similar shot contexts. The workflow includes data preprocessing, visualization, and machine learning models to extract insights from player performance metrics.

## Features
- **Data Cleaning & Preprocessing**: Handles missing values, converts time formats, and removes irrelevant columns.
- **Feature Engineering**: Creates new variables such as `LAST_SHOT` and `CLOSEST_DEFENDER_EFFICIENCY` to enhance analysis.
- **Data Visualization**: Implements histograms, count plots, and heatmaps to explore shooting trends.
- **K-Means Clustering**: Groups similar shot contexts using statistical features.
- **Player Efficiency Adjustment**: Evaluates and ranks players based on shooting performance.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/your-repo/NBA-Shot-Analysis.git
   ```
2. Navigate to the project directory:
   ```sh
   cd NBA-Shot-Analysis
   ```
3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
Run the analysis script using:
```sh
python analysis.py
```
Make sure the dataset (`shot_logs.csv`) is placed in the appropriate directory.

## Technologies Used
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
- **Concepts**: Data Analysis, Clustering, Statistical Modeling

## Implementation Steps
1. **Data Acquisition**: Loads NBA shot log data from `shot_logs.csv`.
2. **Data Cleaning**: Removes unnecessary columns, converts `GAME_CLOCK` to `SECONDS_LEFT_IN_PERIOD`, and fills missing values.
3. **Feature Engineering**: Introduces efficiency-based variables such as `CLOSEST_DEFENDER_EFFICIENCY`.
4. **Data Visualization**: Generates plots to examine distributions and relationships between shooting factors.
5. **Clustering**: Applies K-Means clustering to categorize shots and determines the optimal number of clusters using silhouette scores.
6. **Performance Evaluation**: Adjusts player rankings based on efficiency metrics derived from clustering analysis.


