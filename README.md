# 🚖 Chicago Taxi Rides: Weather Impact Analysis

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=white)

## 📌 Project Overview
This project investigates whether weather conditions (Good vs. Bad) have a statistically significant impact on the duration of taxi rides in Chicago, specifically on the route from **The Loop** to **O'Hare International Airport** on Saturdays.

## 📊 Dataset Structure
The analysis uses the `project_sql_result_07.csv` dataset, which contains:
- `start_ts`: Pickup date and time.
- `weather_conditions`: Description of weather at the start of the ride.
- `duration_seconds`: Total ride duration in seconds.

## 🧪 Hypothesis Testing
We performed an **Independent T-Test** (Welch's T-test) to compare the means of two independent samples:
* **Null Hypothesis (H₀):** The average duration of rides from the Loop to O'Hare is the same regardless of weather conditions.
* **Alternative Hypothesis (H₁):** The average duration of rides changes depending on weather conditions.

### 📈 Results
- **Sample Size (Good Weather):** 888 trips
- **Sample Size (Bad Weather):** 180 trips
- **p-value:** `6.7389e-12`
- **Alpha Level:** 0.05

## 💡 Conclusion
Since the **p-value is significantly lower than 0.05**, we **reject the Null Hypothesis**. There is strong statistical evidence to conclude that weather conditions significantly affect trip durations. Rainy or "Bad" weather Saturdays result in different travel times compared to "Good" weather days.

## 🛠️ How to Run
1. Clone the repository: `git clone https://github.com/SEU-USUARIO/chicago-taxi-analysis.git`
2. Ensure you have the `data/` folder with the CSV file.
3. Install dependencies: `pip install pandas scipy`
4. Run the Jupyter Notebook.

---
*Project developed as part of the TripleTen Data Analytics Bootcamp.*
