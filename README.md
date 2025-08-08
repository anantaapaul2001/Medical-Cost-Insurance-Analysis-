# Medical-Cost-Insurance-Analysis-
**This project aims to analyze and model medical insurance costs based on various personal attributes such as age, BMI, number of children, smoking status, and region. By applying data preprocessing, visualization, and machine learning techniques, we uncover insights and build predictive models to estimate medical charges.**

**📁 Dataset**
The dataset used in this analysis is insurance.csv, which contains the following columns:

1. **age:** Age of the individual
2. **sex:** Gender (male, female)
3. **bmi:** Body Mass Index
4. **children:** Number of dependent children
5. **smoker:** Smoking status (yes, no)
6. **region:** Residential region in the US (northeast, southeast, southwest, northwest)
7. **charges:** Medical insurance cost

**🔧 Tools and Libraries**
1. Python (Pandas, NumPy, Matplotlib, Seaborn)
2. Scikit-learn
3. Jupyter Notebook

**🧼 Data Preprocessing**

1. Checked for missing values and duplicates
2. Encoded categorical variables (sex, smoker, region) using LabelEncoder
3. Copied original dataset to preserve raw data
4. Normalized features where necessary

**📊 Exploratory Data Analysis**
**Key Visualizations:**

- Distribution of charges by smoker/non-smoker
- Violin and box plots of charges segmented by sex and smoking status
- BMI and age distribution
- Scatter plots and regression lines showing relationship between charges, age, and BMI
- Correlation heatmap of all features

**Key Insights:**
- Smokers are charged significantly higher than non-smokers
- BMI and age positively correlate with insurance charges
- Region has negligible effect on charges
- Female smokers tend to have slightly lower charges than male smokers

**🤖 Model Building**

1. Linear Regression
Trained on features like age, sex, BMI, children, smoker, region
_**Test Score (R²): 0.796**_

2. Polynomial Regression (Degree = 2)
Excluded region for better results
Applied PolynomialFeatures transformation
_**Test Score (R²): 0.884**_

Future improvements may include using ensemble methods like Random Forests or Gradient Boosting for enhanced accuracy.

**📈 Conclusion**
**This project successfully demonstrates how basic demographic and lifestyle features can be used to predict medical costs using linear and polynomial regression techniques. It also shows how EDA can uncover strong patterns, especially the impact of smoking on insurance charges.**
