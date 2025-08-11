# 💧 Water Potability Determination

Access to safe drinking water is a fundamental human right, yet **over 2 billion people worldwide** lack access to it.  
Contaminated water can cause severe health issues, including waterborne diseases like cholera, typhoid, and dysentery.  

This project leverages **data science and machine learning** to **predict whether water is safe for human consumption** based on its chemical and physical properties.  
By automating this process, it aims to assist **environmental agencies, researchers, and policymakers** in quickly identifying unsafe water sources — helping reduce health risks and improve public health outcomes.

---

## 📌 Project Overview
The project follows a **structured data science pipeline**:
1. **Data Cleaning & Preprocessing**  
   - Handling missing values using **median imputation** separately for each potability class.  
   - Removing duplicate rows (none found in dataset).  
   - Scaling features using **Min-Max Scaler** for normalization.
   
2. **Exploratory Data Analysis (EDA)**  
   - Distribution analysis of features.  
   - Correlation heatmaps to identify relationships between variables.  

3. **Model Training & Evaluation**  
   - Models Used:
     - Logistic Regression
     - Decision Tree Classifier
     - Random Forest Classifier
     - K-Nearest Neighbors (KNN)
     - Naive Bayes
     - Support Vector Classifier (SVC)
     - XGBoost Classifier
     - AdaBoost Classifier
   - Evaluation Metrics:
     - Accuracy
     - Precision
     - Recall
     - F1 Score

4. **Model Comparison**  
   - Performance comparison across models to identify the best-performing algorithm.

---

## 📂 Dataset
The dataset contains **chemical and physical water quality measures** with the target variable `Potability`:
| Feature        | Description |
|----------------|-------------|
| pH             | pH value of water (0–14 scale) |
| Hardness       | Water hardness (calcium carbonate concentration) |
| Solids         | Total dissolved solids in ppm |
| Chloramines    | Amount of chloramines in ppm |
| Sulfate        | Sulfate concentration in mg/L |
| Conductivity   | Electrical conductivity of water |
| Organic_carbon | Amount of organic carbon in ppm |
| Trihalomethanes| Concentration of trihalomethanes in μg/L |
| Turbidity      | Turbidity level (NTU) |
| Potability     | Target variable (1 = drinkable, 0 = not drinkable) |

Dataset Size: **3,276 samples × 10 columns**

---

## ⚙️ Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/water-potability-determination.git
   cd water-potability-determination
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:
   ```bash
   jupyter notebook water_potability_determination.ipynb
   ```

---

## 📊 Results
| Model                | Accuracy | Precision | Recall | F1 Score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | XX%      | XX%       | XX%    | XX%      |
| Decision Tree        | XX%      | XX%       | XX%    | XX%      |
| Random Forest        | XX%      | XX%       | XX%    | XX%      |
| KNN                  | XX%      | XX%       | XX%    | XX%      |
| Naive Bayes          | XX%      | XX%       | XX%    | XX%      |
| SVC                  | XX%      | XX%       | XX%    | XX%      |
| XGBoost              | XX%      | XX%       | XX%    | XX%      |
| AdaBoost             | XX%      | XX%       | XX%    | XX%      |

*(Replace `XX%` with actual results after running the notebook.)*

---

## 📌 Key Learnings
- **Class-wise imputation** helps retain statistical integrity when data distribution differs between classes.
- **Min-Max Scaling** standardizes feature ranges, improving algorithm performance.
- **Ensemble models** (Random Forest, XGBoost) tend to outperform single estimators for this classification problem.

---

## 📜 License
This project is licensed under the MIT License — you are free to use, modify, and distribute it.

---

