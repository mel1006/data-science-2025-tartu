# UK Road Safety – Accident Severity Analysis

### 📊 Project Overview
This project aims to analyze road accident patterns in the **United Kingdom** and identify the key factors influencing **accident severity**.  
The workflow follows a structured data science process — including data understanding, preprocessing, feature engineering, modeling, and evaluation — to transform raw data into actionable road safety insights.

The main goals are:
- To understand **when, where, and under what conditions** road accidents occur.  
- To identify the **factors influencing accident severity**.  
- To build a **predictive model** that classifies accidents as *Slight*, *Serious*, or *Fatal* based on environmental and situational data.

---

### 🗂️ Dataset Information
The data used in this project come from the official  
**[UK Department for Transport – Road Safety Data](https://www.kaggle.com/datasets/tsiaras/uk-road-safety-accidents-and-vehicles?resource=download&select=Accident_Information.csv)**,  
available publicly via **Kaggle**.

- **Source:** Kaggle – UK Department for Transport  
- **File used:** `Accident_Information.csv`  
- **Years selected:** 2012–2017  
- **Records after filtering:** ~830,000  
- **Variables:** 34 (including accident date, time, location, weather, lighting, road surface, casualties, and severity)

Because the dataset exceeds GitHub’s file size limit (700MB+), it is **not stored in this repository**.  
Instead, the dataset can be downloaded directly from Kaggle using the link above.

---

### 🔍 Methods and Tools
- **Programming & Analysis:** Python (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `imbalanced-learn`)  
- **Modeling Techniques:** Random Forest, HistGradientBoosting, Artificial Neural Network (ANN)  
- **Data Preprocessing:** Feature engineering, One-Hot Encoding, normalization, SMOTE balancing  
- **Evaluation Metrics:** Precision, Recall, F1-score, ROC-AUC, Confusion Matrix  
- **Framework:** CRISP-DM (Business → Data → Modeling → Evaluation)  
- **Environment:** Jupyter Notebook, Visual Studio Code  
- **Version Control:** GitHub  
- **Visualization:** Seaborn, Matplotlib (geographical & categorical plots)  

---

### 🧠 Key Steps Completed

1. **Business Understanding**
- Defined project objectives: identify key factors affecting accident severity and build predictive models.  
- Established success metrics based on recall and F1-score for severe/fatal accidents.  

2. **Data Understanding**  
- Collected and inspected raw data from the UK Department for Transport (2012–2017).  
- Verified completeness, removed invalid or missing coordinates, and checked for duplicates and anomalies.  
- Performed exploratory analysis of accident distribution by time, weather, lighting, and road surface.  

3. **Data Preparation**  
- Cleaned data and standardized formats across 34 attributes.  
- Created engineered features (hour bins, weekday/weekend indicator, daylight conditions).  
- Encoded categorical variables using **One-Hot Encoding** and normalized numeric fields.  
- Addressed class imbalance (~1:5 ratio) using **SMOTE** oversampling and undersampling.  

4. **Modeling** 
- Trained and compared **Random Forest**, **HistGradientBoosting**, and **Artificial Neural Network (ANN)** models.  
- Optimized thresholds and hyperparameters to maximize F1-score.  
- Split dataset into **train (70%)**, **evaluation (15%)**, and **test (15%)** subsets for consistent validation.  

5. **Evaluation and Insights**  
- Evaluated model performance using **Precision**, **Recall**, **F1-score**, **ROC-AUC**, and **Confusion Matrices**.  
- Identified top predictive features: *Number of Vehicles, Speed Limit, Urban/Rural Area,* and *Weekend Indicator.*  
- Found that severe accidents occur more frequently on **Fridays** and under **clear weather conditions**.  

6. **Reporting and Visualization**  
- Created visual summaries: geographical accident maps, severity distributions, and feature importances.  
- Compiled findings into a professional **poster** and **README report** for presentation.  


---

   
### 🔄 How to Reproduce

To replicate this analysis:
1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/tsiaras/uk-road-safety-accidents-and-vehicles).  
2. Place the file `Accident_Information.csv` in the `data/` directory.  
3. Run this notebook from start to finish using Python ≥3.10 and a standard data science stack for data preprocessing, visualization, and machine learning(some libraries may need to be installed beforehand)
4. All random seeds are fixed for reproducibility.

---

### 👥 Team (Group 6)
- *Melesse Perschewski*  
- *Kateryna Kantsyr* 
