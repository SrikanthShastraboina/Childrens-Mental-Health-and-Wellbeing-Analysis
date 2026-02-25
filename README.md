# Children’s Mental Health and Wellbeing Analysis

## Overview
This project analyzes the impact of the COVID-19 pandemic lockdowns on children’s mental health and well-being. Using survey data collected from children and their parents, the goal was to identify emotional and behavioral challenges and provide actionable recommendations for improving their well-being.

## Objectives
- Understand the key factors influencing children’s mental health.
- Analyze emotional and behavioral difficulties using statistical and machine learning methods.
- Provide actionable insights and recommendations for policymakers, educators, and caregivers.

## Dataset
The data was collected from surveys filled out by primary school children with parental consent. It included:
- Emotional indicators (e.g., loneliness, worrying).
- Behavioral patterns (e.g., temper loss, shyness).
- General well-being factors (e.g., family relationships, health).

The dataset was anonymized to ensure confidentiality and included responses from both children and their parents.

## Methodology

### 1. Data Preprocessing
- Removed duplicates and irrelevant columns.
- Addressed missing values using mode (categorical) and median (numerical).
- Derived new features such as "Hours of Sleep."

### 2. Exploratory Data Analysis (EDA)
- Correlation heatmaps for identifying relationships between factors.
- Distribution plots for features like sleep and well-being scores.
- Boxplots to explore variability in emotional and behavioral indicators.

### 3. Modeling Techniques
- Balanced dataset using SMOTE to handle class imbalances.
- Models implemented:
  - Logistic Regression
  - Random Forest
  - XGBoost
  - Support Vector Machine (SVM)
- Performed hyperparameter tuning to optimize model performance.

### 4. Feature Importance
- Used SHAP analysis to identify the most impactful features.
- Highlighted emotional and social indicators as critical factors.

## Key Findings
- Emotional challenges like worrying and loneliness were prevalent.
- Behavioral difficulties such as temper loss and shyness impacted academic performance and social interactions.
- General well-being metrics (e.g., family relationships) were strongly correlated.

## Recommendations
- **Emotional Support:** Introduce mindfulness and stress management programs.
- **Behavioral Interventions:** Provide anger management resources and structured routines.
- **Social Engagement:** Encourage peer interaction through safe activities.

## Technologies Used
- Python (Pandas, Scikit-learn, XGBoost, Seaborn, Matplotlib)
- Jupyter Notebook
- SMOTE for handling imbalanced datasets

## Project Structure
```
children-mental-health-analysis/
├── data/
│   ├── raw_data.csv
│   ├── cleaned_data.csv
├── notebooks/
│   ├── data_preprocessing.ipynb
│   ├── eda.ipynb
│   ├── modeling.ipynb
├── reports/
│   ├── eda_summary.pdf
│   ├── model_performance.pdf
├── src/
│   ├── data_cleaning.py
│   ├── feature_engineering.py
│   ├── modeling.py
└── README.md
```

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/children-mental-health-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd children-mental-health-analysis
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter notebooks for preprocessing, EDA, and modeling:
   ```bash
   jupyter notebook
   ```

## Results
The XGBoost model achieved the highest accuracy of 90%, making it the best-performing model for identifying emotional and behavioral challenges.

## Future Work
- Include longitudinal data to track changes over time.
- Explore additional datasets for validation.
- Develop a dashboard for real-time analysis and visualization.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## Acknowledgments
- Data was anonymized and used ethically with parental consent.
- Thanks to the contributors who supported this analysis.

Feel free to reach out with questions or suggestions!
