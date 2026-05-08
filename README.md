# 🏡 California Housing Price Prediction

A beginner-friendly Machine Learning project that predicts median house values across California neighborhoods using the classic **California Housing Dataset**. Three regression models are trained, compared, and visualized end-to-end.

---

## 📌 Project Overview

This project walks through a complete ML pipeline — from raw data to model evaluation — using Python and scikit-learn. It's designed to be readable and educational for anyone starting out in Machine Learning.

**Goal:** Predict the **median house value** (in $100,000s) of a California district based on features like income, location, and housing characteristics.

---

## 📊 Dataset

- **Source:** [California Housing Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html) (via scikit-learn)
- **Samples:** 20,640 California census block groups
- **Features:** 8 input features + 1 target variable

| Feature | Description |
|---|---|
| `MedInc` | Median income of the block group |
| `HouseAge` | Median age of houses |
| `AveRooms` | Average number of rooms per household |
| `AveBedrms` | Average number of bedrooms per household |
| `Population` | Block group population |
| `AveOccup` | Average household occupancy |
| `Latitude` | Geographic latitude |
| `Longitude` | Geographic longitude |
| `MedHouseVal` ⭐ | **Target** — Median house value ($100k) |

---

## 🧠 Models Trained

| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | 0.905 | 0.417 |
| Decision Tree | 0.950 | 0.303 |
| **Random Forest** ✅ | **0.955** | **0.286** |

> **Random Forest** achieved the best performance with an R² of **0.955** and an average prediction error of ~$28,600.

---

## 🔍 Key Findings

- **Median Income** is the strongest predictor of house value
- **Geographic location** (Latitude/Longitude) is the second most important factor — coastal areas command significantly higher prices
- Random Forest outperforms both Linear Regression and Decision Tree by capturing non-linear relationships in the data

---

## 🗂️ Project Structure

```
california-housing-prediction/
│
├── california_housing_model.py   # Main script — full ML pipeline
├── california_housing_report.png # Visualization report
└── README.md                     # You're reading it!
```

---

## ⚙️ Installation & Usage

**1. Clone the repository**
```bash
git clone https://github.com/your-username/california-housing-prediction.git
cd california-housing-prediction
```

**2. Install dependencies**
```bash
pip install scikit-learn pandas numpy matplotlib seaborn
```

**3. Run the model**
```bash
python california_housing_model.py
```

---

## 📈 Visualizations

The report includes:
- 🔥 **Feature Correlation Heatmap** — see which features relate to house value
- 📉 **House Value Distribution** — understand the spread of prices
- 📊 **R² and RMSE Comparison** — compare all three models at a glance
- 🌲 **Feature Importance** — what the Random Forest considers most useful
- 🎯 **Actual vs Predicted Plots** — visualize prediction accuracy per model

---

## 🛠️ Tech Stack

- **Python 3.x**
- [scikit-learn](https://scikit-learn.org/) — ML models & preprocessing
- [pandas](https://pandas.pydata.org/) — data manipulation
- [NumPy](https://numpy.org/) — numerical computing
- [Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/) — visualizations

---

## 🚀 What's Next?

Ideas to extend this project:
- [ ] Hyperparameter tuning with `GridSearchCV`
- [ ] Try XGBoost or LightGBM for even better accuracy
- [ ] Deploy as a web app using Flask or Streamlit
- [ ] Add geographic price maps using Folium

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

Made with ❤️ and Python. Feel free to fork, star ⭐, or open an issue!
