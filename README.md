# task_02_DA
**Exploratory Data Analysis (EDA)**
This project performs Exploratory Data Analysis (EDA) on the Titanic dataset to uncover meaningful business insights, detect patterns, and analyze survival factors.
The goal is to apply industry-standard EDA techniques using Python and visualize findings effectively.

**Dataset Used**
Titanic Dataset(from Kaggle): https://www.kaggle.com/datasets/brendan45774/test-file

**Tools & Libraries**
-Python
-Pandas → Data manipulation & cleaning
-Matplotlib → Data visualization
-Seaborn → Advanced visualization & statistical plots
-Jupyter Notebook → Analysis workflow

**Steps Performed**
- Data Understanding
  .info(), .describe(), .isnull().sum()
  Identified dataset structure, missing values, and summary statistics.
  
-Missing Data Analysis
  Visualized missing values using sns.heatmap()
  Decided handling strategies (drop/impute).

-Univariate Analysis
  Histograms: Age, Fare, SibSp, Parch
  Countplots: Gender, Passenger Class, Embarked Port
  Boxplots: Age vs Survived, Fare vs Survived

-Bivariate & Multivariate Analysis
  Pairplots to explore variable relationships
  Correlation heatmap to detect numeric dependencies

-Grouping & Aggregation
  .groupby() on Gender, Class, Embarked
  Calculated survival rates per category

-Outlier & Skewness Detection
  Checked .skew() for numeric features
  Applied log transformations on Fare, SibSp, Parch to reduce skewness
  Boxplots to visualize outliers

**Key Insights**
-Women had a much higher survival rate than men.
-Higher-class passengers (1st Class) had better chances of survival.
-Fares were heavily skewed; log transform improved normality.
-Most passengers had no siblings/spouse or parents onboard (skewed family features).
