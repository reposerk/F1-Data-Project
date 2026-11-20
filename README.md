# F1 Performance Analytics & Predictive Modeling

A Python data analytics project that processes, and analyzes Formula 1 telemetry data from the Ground Effect era, collected from the  **FastF1 API**. It transforms lap-by-lap race records into driver-level summaries to evaluate the statistical impact of qualifying position, tire strategy, and speed on final race outcomes.

## How to Use

1. **Clone the repository:**
   ```bash
   git clone https://github.com/reposerk/F1-Data-Project.git
   cd F1-Data-Project
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas numpy fastf1 scikit-learn matplotlib seaborn
   ```

3. **Run the pipeline & analysis (in 'Project Code Dump.ipynb':**
   * Run data preprocessing scripts (or use the provided csv files) to pull season telemetry and build the aggregated dataset.
   * Visualize the data with correlation matrices and heat maps.
   * Execute the modeling scripts to generate various models, including linear regression and neural networks.

## Example Results

* **Feature Engineering:** Aggregated driver records across three seasons, converting raw lap-by-lap timing and categorical tire compounds into usage metrics, cumulative stint lengths, and pit-stop deltas.
* **Key Statistical Findings:** 
  * **Qualifying Dominance:** Starting grid position showed the strongest positive correlation with final finishing position across the dataset.
  * **Tire Strategy Impact:** Regression analysis highlighted that optimizing stint lengths and minimizing pit-stop time loss yielded measurable position gains, particularly on high-degradation circuits.
