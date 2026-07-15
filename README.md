# VortexTech Data Science Internship — Week 2: Exploratory Data Analysis with Insights

## What this project does
This project builds on the Week 1 cleaned dataset to run a structured exploratory data analysis (EDA):
- Correlation matrix and heatmap across all numeric columns
- Scatter plots for the two strongest numeric relationships
- A grouped categorical comparison (average tip percentage by day)
- 3 specific, data-backed insights, each supported by its own chart

## Dataset
`restaurant_tips_raw.csv` — same raw restaurant visit dataset used in Week 1 (250 rows; a quick recap clean is re-applied at the top of the notebook).

## Files
- `week2_eda_with_insights.ipynb` — the main notebook (already executed, with all outputs and charts visible)
- `restaurant_tips_raw.csv` — the raw dataset used

## How to run
1. Clone this repository.
2. Install the required libraries:
   ```
   pip install pandas matplotlib seaborn jupyter
   ```
3. Launch Jupyter and open the notebook:
   ```
   jupyter notebook week2_eda_with_insights.ipynb
   ```
4. Run all cells from top to bottom (`Cell → Run All`).

## Key insights
1. **Total bill is the strongest driver of tip amount** (correlation ≈ 0.67) — bigger checks reliably produce bigger tips, across both lunch and dinner.
2. **Party size mainly explains bill size, not tipping generosity** (correlation between size and total bill ≈ 0.59) — larger groups spend more, but that's a volume effect, not extra generosity per dollar.
3. **Saturday has the most visits but the lowest average tip percentage (~15%), while Friday tips the highest (~17%)** — customer volume and customer generosity are two separate patterns.
