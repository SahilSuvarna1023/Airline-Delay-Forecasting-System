
# ✈️ Airline Delay Forecasting System

This project aims to predict **flight delays** using real-world US domestic airline data.  
We use SQL for exploratory analysis and Random Forest models for both **multiclass** and **binary classification** of delay outcomes.

---

## 📌 Objective

Build a machine learning pipeline to classify flights as:
- ✅ **On-time**
- ⚠️ **Minor Delay**
- 🚨 **Major Delay**

And compare performance against a simplified **binary classification** (delayed or not).

---

## 📂 Dataset

- **Source**: U.S. Domestic Flights (2018–2024)
- **Hosted on Kaggle**:  
  👉 [Kaggle Dataset: U.S. Flight Delay Data (2018–2024)](https://www.kaggle.com/datasets/shubhamsingh42/flight-delay-dataset-2018-2024)  
  *(Note: You’ll need to manually download due to GitHub’s 100MB file limit.)*


---

## 🛠️ Tech Stack

| Tool          | Purpose                         |
|---------------|----------------------------------|
| Python        | Core programming                |
| Pandas        | Data manipulation               |
| DuckDB (SQL)  | Exploratory data analysis       |
| Scikit-learn  | Machine learning models         |
| Git LFS       | Large file tracking (for models)|
| Google Colab  | Development environment         |

---

## 📊 Modeling Approach

We trained and evaluated two model variants:

### ✅ Binary Classification

| Metric   | Value |
|----------|--------|
| Accuracy | 0.59   |
| F1 Score | 0.50   |
| AUC      | 0.61   |

✅ Best for real-world use: simple, reliable predictions for “delayed or not.”

### 🟨 Multiclass Classification

| Class         | F1 Score |
|---------------|----------|
| On-time       | 0.63     |
| Minor Delay   | 0.25     |
| Major Delay   | 0.30     |
| Accuracy      | 0.47     |

🧪 Insight: more granular but suffers from **class imbalance** and reduced recall.

---

## 📈 Visual Results

- ✅ Confusion matrices
- ✅ ROC curve (binary model)
- ✅ Feature importance
- ✅ Class distribution plots

<p align="center">
  <img src="output/Binary Classifier - Confusion Matrix.png" width="350"/>
  <img src="output/ROC Curve.png" width="350"/>
</p>

---

## 📁 Project Structure
Airline-Delay-Forecasting-System/
├── data/ # Dataset folder (user downloads from Kaggle)
├── output/ # Model outputs, plots
├── notebooks/ # Jupyter notebooks (EDA, training)
├── Mark42.ipynb # Final ML pipeline
├── README.md # Project documentation


---

## 🧠 What We Learned

- **Binary classification** is better for alert systems
- **Multiclass adds granularity**, but requires more balanced data
- Preprocessing and SQL exploration help expose key trends (e.g., peak delay times)

---

## 🚀 Future Improvements

- Add **weather and holiday** data
- Use **XGBoost** or **LightGBM**
- Deploy with **Streamlit dashboard** or **API**

---

## 📜 License

This project is for educational and research use.

---

## 🙌 Credits

- Dataset: [Bureau of Transportation Statistics](https://www.transtats.bts.gov/)
- Tools: Python, DuckDB, scikit-learn, Git LFS




