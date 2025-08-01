# project-ml-house-pricing


**Context**
This project aims to estimate house prices using a supervised machine learning approach. We explored the impact of multiple property features—including size, location, and condition—on housing prices. Our goal was to build an accurate and explainable regression model to predict real estate value.

The project was carried out as part of a short data science sprint by a team of four, combining data analysis, feature engineering, and model experimentation.



**🎯Prediction**

Predict the price of a house based on features like surface area, number of bathrooms, location (zipcode), etc.

The target variable is continuous, making this a regression problem.


- 🛠 GitHub Repository: [project-ml-house-pricing](https://github.com/JujuGnirt/project-ml-house-pricing)
- 📋 Trello Board: [Project Tasks & Timeline](https://trello.com/b/FMGH2mNw/ml-house-pricing)
- Presentation: [Canva] https://www.canva.com/design/DAGupoMTRuI/LrJn_LhgrqEjyGea4UsNZQ/edit?utm_content=DAGupoMTRuI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton 

---

# Main dataset issues

Presence of outliers in features like sqft_living and price

Missing values in certain features

Zip codes are categorical but need numerical representation for regression

Correlation between features.

# Solutions for the dataset issues

Dropped irrelevant columns (e.g., id, date, etc.)

Encoded zipcode using a ratio-based transformation tied to average house price

Removed outliers based on domain knowledge and percentile filtering

Checked correlation both linearly and non-linearly (e.g., Pearson + heatmaps) 

# Models Tested

Model                   Performance (R² on Test)
K-Nearest Neighbors        0.49
Decision Tree              0.72
Random Forest              0.78

# Insights 

sqft_living, grade, and bathrooms were among the most important features driving price.

A custom transformation on zipcode helped reduce its categorical noise and made it more informative.

# Futur Works and Improvement

Spend more time on cross-validation
Using Relative Error instead of Absolute so our range of error correspond to the price we predict
Include time-related variables (year sold, seasonality)
Incorporate external data (schools, crime rates, transport)

# Repository Structure

```

ml-house-pricing/
├── data/                        # Raw and cleaned CSV files
├── notebooks/                   # Python notebooks with analysis
├── slides/                      # Presentation
├── README.md                    # Introduction of the purpose of this project
├── .gitignore                   # 
├── 

```


##  Tools Used
 
- Python (Pandas, sklearn)  
- Jupyter Notebooks  
- Git & GitHub  
- Trello (for task planning)  
- Visual Studio Code IDE & plugins
  
---

## 👥 Team Members

__* Adam Askari,
Macarena Ruiz,
Damian Witowski,
Julie Tring
*__