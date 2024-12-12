# INST462-Umpire

This project focuses on analyzing MLB umpire data to uncover insights about their performance, consistency, and biases. The project is divided into two main scripts: a data cleaning script and a visualization script.

---

## Data Cleaning Script (`clean.py`)
### Purpose:
The data cleaning script prepares raw MLB umpire data for analysis by performing the following steps:
1. **Loading Data**: Reads the raw CSV file.
2. **Cleaning**:
   - Handles missing values.
   - Converts relevant columns to appropriate data types (e.g., numeric, datetime).
   - Removes duplicate rows.
3. **Saving**:
   - Outputs a cleaned CSV file ready for analysis.

### Usage:
Run this script to transform the raw dataset into a clean, structured format. The cleaned dataset will be saved as `MLB_Umpire_Cleaned_Data.csv` in the specified directory.

---

## Visualization Script (`visualize_mlb_data.py`)
### Purpose:
The visualization script generates insightful graphs to explore relationships and patterns in the cleaned data. It produces the following visualizations:
1. **Distribution of Umpire Accuracy**:
   - A histogram showing the distribution of accuracy percentages.
2. **Incorrect Calls vs. Total Run Impact**:
   - A scatterplot visualizing how incorrect calls relate to total run impact, colored by home team bias.
3. **Correct Calls vs. Favor Home**:
   - A scatterplot highlighting the relationship between correct calls and home team favorability.
4. **Umpire vs. Accuracy**:
   - A boxplot showcasing accuracy distributions for individual umpires.
5. **Home vs. Favor Home**:
   - A boxplot analyzing the relationship between home teams and favorability.

### Usage:
Run this script to generate and save visualizations as PNG files in the output directory. Each graph is designed to provide a unique perspective on umpire performance metrics.

---

## Requirements
- **Python 3.x**
- Libraries:
  - `pandas`
  - `matplotlib`
  - `seaborn`

### Running the Scripts:
1. Place the raw data file (`MLB_Umpire_Raw_Data.csv`) in the specified directory.
2. Run the cleaning script:
   ```bash
   python clean.py
   ```
3. Run the visualization script:
   ```bash
   python visualize_mlb_data.py
   ```

---

## Output
- **Cleaned Data**: `MLB_Umpire_Cleaned_Data.csv`
- **Graphs**:
  - `distribution_of_umpire_accuracy.png`
  - `incorrect_calls_vs_total_run_impact.png`
  - `correct_calls_vs_favor_home.png`
  - `umpire_vs_accuracy.png`
  - `home_vs_favor_home_boxplot.png`

