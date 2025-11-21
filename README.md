# 📘 World Happiness Analysis (2015–2021)

This project explores global happiness trends using the **World Happiness Report** dataset. It focuses on understanding how key socioeconomic factors influence happiness and uses a linear regression model to predict happiness scores for future years (2020 and 2021).

The analysis includes:
- Data preprocessing and cleaning  
- Statistical analysis  
- Visualisation of global well-being indicators  
- Machine learning model development  
- Predictions and accuracy evaluation for 2020 and 2021  

---

## 🌍 Dataset Source

This project uses the following Kaggle dataset:

### **World Happiness Report (till 2023)**  
🔗 https://www.kaggle.com/datasets/sazidthe1/global-happiness-scores-and-factors/data

The dataset includes country-level indicators such as:
- Happiness Score / Life Ladder  
- GDP per capita  
- Social support  
- Healthy life expectancy  
- Freedom to make life choices  
- Generosity  
- Perceptions of corruption  
- Regional classifications  

CSV files for the years **2015–2023** are provided.  
This project specifically uses **2015–2021**.

---

## 📂 Project Structure

```
DataScience-World-Happiness-Analysis/
│
├── notebook.ipynb                # Main Jupyter Notebook (full analysis)
├── notebook.txt                  # Code-only version (for assessment submission)
│
├── WHR_2015.csv
├── WHR_2016.csv
├── WHR_2017.csv
├── WHR_2018.csv
├── WHR_2019.csv
├── WHR_2020.csv
├── WHR_2021.csv
│
└── README.md                     # Project documentation
```

---

## 🧪 Methods

### **1. Data Preparation**
- Standardised inconsistent column names  
- Selected common features across years  
- Merged all years into one dataset  
- Handled missing values using median imputation  
- Ensured the dataset followed First Normal Form (1NF)  
- Optional: Applied data normalisation  

### **2. Statistical Analysis**
- Mean, median, and standard deviation  
- Variance, skewness, and kurtosis  
- Understanding distribution patterns of each feature  

### **3. Visualisation**
- Correlation heatmap  
- Scatterplots: GDP, social support, life expectancy vs happiness  
- Histogram of happiness score distribution  

### **4. Linear Regression Model**
Features used:
- GDP per capita  
- Social support  
- Healthy life expectancy  
- Freedom to make life choices  
- Generosity  
- Perceptions of corruption  

Model evaluation metrics:
- **R² score**
- **RMSE (Root Mean Squared Error)**

### **5. Predictions for 2020 and 2021**
The model trained on 2015–2019 was used to forecast happiness scores for later years.

**2020 Accuracy**  
- RMSE: **0.568**  
- MAPE: **9.01%**  
- Accuracy: **90.99%**

**2021 Accuracy**  
- RMSE: **0.593**  
- MAPE: **9.14%**  
- Accuracy: **90.86%**

These results show strong model performance and consistent predictive ability.

### **6. Feature Engineering**
Explored:
- Polynomial features (degree 2)  
- Interaction terms  
- Re-evaluated the model for performance changes  

---

## 📈 Summary of Findings

- Socioeconomic indicators such as **GDP**, **social support**, and **life expectancy** are the strongest predictors of happiness.  
- Linear regression provides a clear and interpretable model with high accuracy.  
- Predictions for 2020 and 2021 demonstrate strong generalisation despite real-world disruptions (e.g., COVID-19).  
- Feature engineering can slightly improve performance but also increases model complexity.  

---

## 🚀 How to Run the Project

### Install required packages:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Launch Jupyter Notebook:
```
jupyter notebook
```

Open:

```
notebook.ipynb
```

Run all cells in order.

---

## 🙌 Acknowledgements

- **Dataset:** World Happiness Report (Kaggle)  
- **Dataset Author:** Sazid Mahmud  
- https://www.kaggle.com/datasets/sazidthe1/global-happiness-scores-and-factors/data  
- **Analysis & modelling:** Linear regression using scikit-learn  

---

## 📜 License

This project uses publicly available data from Kaggle and is for academic and educational purposes.
