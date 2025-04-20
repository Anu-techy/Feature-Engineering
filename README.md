**Feature Engineering** is the process of creating, transforming, or selecting input variables (features) from raw data to improve the performance of machine learning models.
It is done using Business understanding or statistics.

**Why It Matters:**

Better features = Better model performance 

It helps models understand patterns more clearly and make more accurate predictions.

**Key Steps in Feature Engineering:**

Remove duplicates, 

treat outliers

Creating new features   ---	Combine "date of birth" and "current date" to create "age"

Transforming data	Log   ---  transform highly skewed features (e.g., income)

Encoding categorical vars  --  	Convert "City = Mumbai" into one-hot or label encoding

Scaling features	----   Normalize values ( from dollars to INR)

Handling missing values	--   Fill missing "age" with average or use model-based imputation

Feature selection	--  Keep only the most relevant features to reduce noise

=====================================================================

**Feature Selection using Correlation**

For non linear relationships , one should not use correlation for feature selection

In the presence of outliers, one should not use correlation for feature selection

For categorical variables, correlation should not be used for feature selection     

Understand r/p b/w causation vs correlation

=====================================================

**Multicollinearity** occurs when two or more independent variables (features) in a regression model are highly correlated with each other.

In simple terms: the model is getting the same information from multiple features, which confuses it.**

**Cons of Multicollinearity**

Reduces model interpretability	Hard to tell which variable is actually affecting the output

Inflates standard errors	Makes coefficients less reliable (can flip signs or seem insignificant)

Causes unstable predictions	Small changes in data can cause big changes in model output

**How to find multicollinearity**

Correlation Matrix	Checks pairwise correlation between features

VIF (Variance Inflation Factor)	Measures how much a feature is correlated with others — VIF > 5 or 10 is a red flag

============================================================================

**Feature Selection using VIF(Variance Inflation Factor)**

VIF = 1 / (1-R sqr)   

if vif =1 , no correclation

if vif is large, strong correlation

vif>10 not recommended

Remove the features with high vif one by one
