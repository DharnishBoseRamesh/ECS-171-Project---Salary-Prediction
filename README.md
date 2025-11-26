# ECS-171-Project---Salary-Prediction

## Description
Our project is about building a machine learning model to predict salaries based on factors such as job title, years of experience, education, cost of living, location, and many more features. The goal is to create a reliable model that can provide salary estimates for different job positions. We will use a publicly available dataset (most likely from Kaggle) containing job data with the features listed above. Our approach will be testing different regression models such as linear regression, polynomial regression, decision tree regression, random forest regression and other methods as well. This project is significant because it will help job seekers and employers understand compensation trends and set expectations. The results will include model performance metrics, feature importance analysis, a comparison of different models, and salary predictions for new data based on job title, experience, and other factors.

## Installation and Deployment Instructions 
* Python 3.10+ recommended 
* Required Packages: NumPy, Pandas, Matplotlib, SciPy, scikit-learn, notebook

```bash
pip3 install numpy pandas matplotlib scipy scikit-learn notebook
python3 -m notebook
```
Project Files
* Gradient Boosting code in code/gradient_boosting.ipynb 
* OLS code in code/Linear_Regression_OLS.ipynb 
* Gradient Descent code in code/Salary-Prediction-Using-LR-GD.ipynb

## Data Cleaning and Exploratory Data Analysis (Louyang Pang)
Data Cleaning
1. Remove duplicate data by eliminating identical rows to prevent statistical bias.  
2. Handle missing values:  
   - Fill numeric columns with the median.  
   - Replace categorical columns with Unknown.  
3. Outlier Removal:  
   Remove extreme salary data using the Interquartile Range (IQR) method  
4. Save the cleaned dataset: 
   `data/process/clean_salary_data.csv`

Exploratory Data Analysis
1. Visualize the cleaned salary distribution.  
2. Compare salary differences by education level (Salary by Education Level)  
3. Analyze the most common job titles (Top Job Titles)  
4. Plot a correlation heatmap (Correlation Heatmap) to observe relationships between salary and features like experience  
5. Save all charts to:  
   `reports/figures/`
(ignore ai_job_salary_2025.csv and clean_ai_salary_2025, they only include ai jobs.)
