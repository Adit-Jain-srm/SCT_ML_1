# SCT_ML_1 - Machine Learning Internship Projects

## 📋 Internship Information
**Intern:** Adit Jain  
**Intern ID:** SCT/JUL25/2512  
**Email:** aj9104@srmist.edu.in  
**LinkedIn:** [www.linkedin.com/in/-adit-jain](https://www.linkedin.com/in/-adit-jain)  
**Company:** SkillCraft Technology  
**Repository:** SCT_ML_1  

---

## 📊 Task 1: House Price Prediction using Linear Regression

### 🎯 Objective
Implement a linear regression model to predict house prices based on:
- **Square footage** (living area)
- **Number of bedrooms**  
- **Number of bathrooms**

### 📁 Project Structure
```
SCT_ML_1/
├── House Prices Data/
│   ├── train.csv                    # Training dataset (1460 samples, 81 features)
│   ├── test.csv                     # Test dataset (1459 samples)
│   ├── data_description.txt         # Feature descriptions
│   └── sample_submission.csv        # Sample submission format
├── linear_regression_house_prices.ipynb  # Main implementation notebook
├── requirements.txt                 # Python package dependencies
└── README.md                        # Project documentation
```

### 🔧 Technologies Used
- **Python 3.8+**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **scikit-learn** - Machine learning library
- **matplotlib** - Data visualization
- **seaborn** - Statistical data visualization
- **jupyter** - Interactive notebook environment
- **scipy** - Scientific computing

*All dependencies are listed in `requirements.txt` for easy installation*

### 📈 Features Engineering
1. **Square Footage**: `GrLivArea` (Above grade living area in sq ft)
2. **Bedrooms**: `BedroomAbvGr` (Number of bedrooms above basement level)
3. **Total Bathrooms**: Combined feature from:
   - `FullBath` (Full bathrooms above grade)
   - `HalfBath` (Half bathrooms above grade × 0.5)
   - `BsmtFullBath` (Basement full bathrooms)
   - `BsmtHalfBath` (Basement half bathrooms × 0.5)

### 🚀 Implementation Highlights

#### Data Preprocessing
- Handled missing values in bathroom counts
- Created engineered feature for total bathrooms
- Applied feature standardization using `StandardScaler`
- Split data into 80% training and 20% testing sets

#### Model Training
- **Algorithm**: Linear Regression
- **Features**: 3 carefully selected predictors
- **Scaling**: Standardized features for optimal performance
- **Validation**: Train-test split with random_state=42

#### Model Evaluation Metrics
- **R-squared (R²)**: Coefficient of determination
- **Root Mean Squared Error (RMSE)**: Prediction accuracy
- **Mean Absolute Error (MAE)**: Average prediction error
- **Residual Analysis**: Model assumption validation

### 📊 Key Results
- ✅ Successfully implemented linear regression model
- ✅ Achieved good predictive performance on test set
- ✅ Identified living area as the strongest price predictor
- ✅ Provided interpretable coefficients for business insights
- ✅ Generated example predictions for different house configurations

### 🔍 Model Interpretation
The linear regression equation provides clear insights:
- **Living Area**: Each additional sq ft increases price by $X
- **Bathrooms**: Each additional bathroom increases price by $Y  
- **Bedrooms**: Each additional bedroom affects price by $Z

*Note: Exact coefficient values are calculated in the notebook execution*

### 📝 Usage Instructions

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd SCT_ML_1
   ```

2. **Install required packages**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**:
   ```bash
   jupyter notebook linear_regression_house_prices.ipynb
   ```

4. **Execute cells sequentially** to:
   - Load and explore the dataset
   - Perform feature engineering
   - Train the linear regression model
   - Evaluate model performance
   - Generate predictions

### 📚 Dataset Information
- **Source**: House Prices Dataset
- **Training Samples**: 1,460 houses
- **Features**: 81 columns (using 3 key features)
- **Target Variable**: `SalePrice` (house sale price in dollars)
- **Evaluation Metric**: RMSE on logarithmic scale

### 🎯 Learning Outcomes
1. **Data Preprocessing**: Handling missing values and feature engineering
2. **Linear Regression**: Understanding coefficients and model interpretation
3. **Model Evaluation**: Using multiple metrics for comprehensive assessment
4. **Data Visualization**: Creating informative plots for analysis
5. **Predictive Modeling**: Making predictions on new data

### 🔗 Additional Resources
- [Scikit-learn Linear Regression Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
- [House Prices Dataset Description](./House%20Prices%20Data/data_description.txt)
- [Python Package Requirements](./requirements.txt)

---

## 📈 Future Tasks
*Additional machine learning tasks will be documented here as they are completed during the internship.*

---

## 📞 Contact
For questions or feedback regarding this project:
- **Email**: aj9104@srmist.edu.in
- **LinkedIn**: [Adit Jain](https://www.linkedin.com/in/-adit-jain)

---

**© 2025 - SkillCraft Technology ML Internship | Task 1 Completed**