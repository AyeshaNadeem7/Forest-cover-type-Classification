# Forest-cover-type-Classification
Build a machine learning model to predict the type of forest cover (tree species category) for a given geographical location based on environmental and cartographic features. This helps automate forest classification and supports ecological planning, wildfire risk analysis, and forest management.

📦 Dataset:
The dataset was obtained from Kaggle (originally from the UCI Machine Learning Repository). It includes 581,012 records with various topographic, hydrologic, and soil features collected from the Roosevelt National Forest in Colorado, USA.

As the data Set is too large so cannot be uploaded in this repository .
If you want to review the dataset follow the link: https://www.kaggle.com/datasets/uciml/forest-cover-type-dataset

🎯The target variable is Cover_Type, a multiclass variable with 7 forest types (e.g., Spruce/Fir, Lodgepole Pine, Aspen, etc.)

🛠 Data Preprocessing:

Cleaned data (no missing values originally)

Standardized column names for readability

Scaled numerical features using StandardScaler


📊 Exploratory Data Analysis (EDA):
Analyzed class distribution (slight imbalance, e.g., rare classes like Cover Type 4)

Plotted correlation heatmaps to check inter-feature relationships

Found Elevation, Soil_Type, and Horizontal_Distance_To_Roadways highly correlated with forest cover type

🤖 Model Building & Evaluation
Two machine learning models were trained and compared:

🌳 Random Forest Classifier
Ensemble of decision trees using bagging

High accuracy and generalization

Handled class imbalance better

🧾 Performance:

🔹 Accuracy: 95.07%

🔹 Excellent precision and recall across all classes

🔹 Best at predicting rare classes (like Cover_Type 3 & 4)

⚡ XGBoost Classifier
Gradient boosting decision trees

Faster, highly tunable, and optimized

More sensitive to class imbalance

🧾 Performance:

🔹 Accuracy: 86.93%

🔹 Good on common classes, weaker on rare classes

🔹 Benefit from hyperparameter tuning

📌 Key Insights:
Elevation, Soil Type, and Horizontal Distance to Roads were the most influential features

Random Forest outperformed XGBoost in overall accuracy and class balance

XGBoost can improve significantly with class weighting or hyperparameter tuning

Predictions may vary between models for borderline or rare class inputs

🧠 Technologies Used:

🐍 Python 

📊 Pandas, NumPy (data handling)

⚙️ Scikit-learn (Random Forest, preprocessing)

🚀 XGBoost (advanced boosting model)

📈 Matplotlib, Seaborn (EDA & visualizations)
