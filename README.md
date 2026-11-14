# F1 Performance Analytics & Predictive Modeling

A Python data analytics project that uses the **FastF1 API** to collect, process, and analyze Formula 1 telemetry data from the Ground Effect era. It transforms lap-by-lap race records into driver-level summaries to evaluate the statistical impact of qualifying position, tire strategy, and speed on final race outcomes.

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/f1-performance-analytics.git
   cd f1-performance-analytics
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas numpy fastf1 scikit-learn matplotlib seaborn
   ```

3. **Run the pipeline & analysis:**
   * Run the data ingestion and feature engineering scripts (or open the Jupyter Notebooks in `notebooks/`) to pull season telemetry and build the aggregated dataset.
   * Execute the modeling script to generate correlation matrices and linear regression outputs.

## Example Results

* **Feature Engineering:** Successfully aggregated 900+ multi-season driver records, converting raw lap-by-lap timing and categorical tire compounds into percentage-wear metrics, cumulative stint lengths, and pit-stop deltas.
* **Key Statistical Findings:** 
  * **Qualifying Dominance:** Starting grid position showed the strongest positive correlation with final finishing position across the dataset.
  * **Tire Strategy Impact:** Regression analysis highlighted that optimizing stint lengths and minimizing pit-stop time loss yielded measurable position gains, particularly on high-degradation circuits.