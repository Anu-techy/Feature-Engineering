**Feature Engineering** is the process of creating, transforming, or selecting input variables (features) from raw data to improve the performance of machine learning models.

**Why It Matters:**

Better features = Better model performance 

It helps models understand patterns more clearly and make more accurate predictions.

**Key Steps in Feature Engineering:**

Creating new features   ---	Combine "date of birth" and "current date" to create "age"

Transforming data	Log   ---  transform highly skewed features (e.g., income)

Encoding categorical vars  --  	Convert "City = Mumbai" into one-hot or label encoding

Scaling features	----   Normalize values (e.g., salary from ₹10k to ₹1L → scaled to 0–1 range)

Handling missing values	--   Fill missing "age" with average or use model-based imputation

Feature selection	--  Keep only the most relevant features to reduce noise
