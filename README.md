# 🚖 Predictive Taxi Insights: Chicago Weather Impact Analysis

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

## 📌 Project Overview
This project performs an end-to-end data analysis to investigate how weather conditions affect urban mobility in Chicago. Using SQL-extracted datasets and Python statistical libraries, we analyze taxi trip durations from **The Loop** to **O'Hare International Airport** on Saturdays.

## 📂 Project Structure
To maintain a clean and professional environment, the repository is organized as follows:
- `notebooks/`: Contains the Jupyter Notebook (`notebook_en.ipynb`) with the full analysis.
- `data/`: Contains the raw datasets used for the study.
- `Images/`: Visualizations and plots generated during the EDA.

## 🧪 Statistical Hypothesis Testing
The core of this project is a formal hypothesis test to determine if "Bad" weather (rain/storm) significantly changes ride durations compared to "Good" weather.

* **Null Hypothesis (H₀):** The average duration of rides from the Loop to O'Hare remains the same regardless of weather conditions.
* **Alternative Hypothesis (H₁):** The average duration of rides changes depending on weather conditions.
* **Test Type:** Independent T-Test (Welch's T-test) with $\alpha = 0.05$.

### 📊 Results & Technical Findings
The analysis yielded the following results:
- **Sample Size (Good Weather):** 888 trips
- **Sample Size (Bad Weather):** 180 trips
- **p-value:** `6.7389e-12`

**Conclusion:** Since the **p-value is significantly lower than 0.05**, we **reject the Null Hypothesis**. There is strong statistical evidence to conclude that weather conditions significantly impact trip durations, likely due to traffic congestion and reduced speed during rainy Saturdays.

## 🛠️ How to Use
1. **Clone the repository:**
   ```bash
   git clone https://github.com/rogeriobarberi-sys/predictive-taxi-insights.git
