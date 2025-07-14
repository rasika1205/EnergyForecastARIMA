---

# Energy Demand Forecasting with ARIMA

Forecasting energy demand is crucial for grid stability, planning, and the integration of renewable energy sources. This project demonstrates how to use the **ARIMA (AutoRegressive Integrated Moving Average)** model for univariate time series forecasting, specifically targeting Italy’s hourly energy load data. The approach leverages modern Python data science tools and showcases a practical workflow from exploratory analysis to final forecasting.

---

## 📌 Objective

- **Forecast** future energy demand using historical load data.
- **Analyze** seasonal and trend patterns in energy consumption.
- **Demonstrate** the effectiveness of ARIMA for time series forecasting.
- **Visualize** findings for clear communication and insights.

---

## 📊 Dataset

- **Source**: Hourly CSV data (2016) containing:
  - `utc_timestamp`: Coordinated Universal Time for each record.
  - `IT_load_new`: Hourly energy load (MW) for Italy.
  - `IT_solar_generation`: Hourly solar generation (MW) for Italy.
- **Note:** Dataset should be placed in the project directory.

---

## 🔧 Tools & Technologies

- **Programming Language**: Python 3.x
- **Notebook Interface**: Jupyter Notebook
- **Data Manipulation**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Time Series Modeling**: statsmodels (ARIMA)
- **Other dependencies**: scipy, warnings

---

## 🛠️ Project Workflow

1. **Data Loading & Preprocessing**
   - Import CSV, parse timestamps, handle missing values.
   - Set `utc_timestamp` as time-series index.

2. **Exploratory Data Analysis**
   - Visualize load and solar generation trends.
   - Identify seasonality, outliers, and missing data.

3. **Time Series Decomposition**
   - Use statistical methods to separate trend, seasonality, and noise.

4. **ARIMA Modeling**
   - Check stationarity and perform differencing if needed.
   - Select model parameters (p, d, q) using ACF/PACF plots.
   - Fit ARIMA model to `IT_load_new` series.

5. **Forecasting & Evaluation**
   - Generate forecasts for future time intervals.
   - Visualize actual vs forecasted values.
   - Evaluate with metrics such as MAE, RMSE.

6. **Interpretation & Insights**
   - Discuss findings, limitations, and potential improvements.

---

## 📁 Repository Structure

```
EnergyForecastARIMA/
│
├── Energy Demand Forecasting with ARIMA.ipynb  # Main notebook with code and explanations
├── energy_dataset_2016.csv                     # Example dataset (not included for copyright reasons)
├── README.md                                   # Project documentation (this file)
└── requirements.txt                            # List of Python dependencies
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/rasika1205/EnergyForecastARIMA.git
cd EnergyForecastARIMA
```

### 2. Install dependencies

We recommend using a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Download the dataset

Place your dataset (e.g., `energy_dataset_2016.csv`) in the project directory.

### 4. Run the notebook

```bash
jupyter notebook "Energy Demand Forecasting with ARIMA.ipynb"
```

---

## 📈 Sample Results

Plots and results in the notebook include:
- Time series plots of energy load and solar generation
- Predicted vs actual load for selected time periods
- Evaluation metrics (e.g., MAE, RMSE)

---

## 💡 Future Work

- Integrate multivariate models (e.g., include weather variables)
- Experiment with other forecasting algorithms (SARIMA, LSTM)
- Automate hyperparameter tuning
- Deploy as a web service or dashboard for real-time forecasting

---


## 📄 License

This project is **proprietary** and protected by copyright © 2025 Rasika Gautam.

You are welcome to view the code for educational or evaluation purposes (e.g., portfolio review by recruiters).  
However, you may **not copy, modify, redistribute, or claim this project as your own** under any circumstances — including in interviews or job applications — without written permission.

---

Feel free to explore the code.

_Developed with 💡 by [Rasika Gautam](https://github.com/rasika1205)_

## 🙏 Acknowledgements

- ARIMA methodology: [Statsmodels Documentation](https://www.statsmodels.org/)
- Visualization inspirations: matplotlib, seaborn communities

---
