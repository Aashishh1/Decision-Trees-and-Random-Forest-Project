<div align='center'>
  <img style="width:30%" src='https://github.com/user-attachments/assets/077dfbe1-393d-4637-a068-8d137cfee83a'/>
</div>

<div align='center'> 
  <h1> Decision Trees and Random Forest Project </h1> 
</div>

This project applies **Decision Trees and Random Forest** algorithms to predict whether a borrower will fully repay a loan using LendingClub data (2007-2010). The model aims to assist investors in making informed lending decisions based on borrower profiles. The dataset contains loan-related features that influence repayment behavior, and this project explores how machine learning models can classify loan repayment risk.

## 🛠️ Technologies Used
- **Python**
- **Scikit-learn**
- **Pandas & NumPy**
- **Matplotlib & Seaborn**
- **Jupyter Notebook**


## 🔍 Methodology

| Phase | Step | Description |
|------|------|------------|
| **Data Preprocessing** | Handling Missing Values | Checked the dataset for missing values and handled them using appropriate imputation techniques. |
|  | Encoding Categorical Variables | Converted the `purpose` feature into dummy variables using one-hot encoding. |
|  | Feature Scaling | Standardized numerical features such as `int.rate` and `installment` to improve model performance. |
|  | Train-Test Split | Split the dataset into **80% training data** and **20% testing data**. |
| **Exploratory Data Analysis (EDA)** | Loan Repayment Distribution | Visualized the proportion of fully paid vs. not fully paid loans. |
|  | FICO Score Analysis | Analyzed the relationship between FICO credit scores and loan repayment behavior. |
|  | Correlation Analysis | Examined correlations among numerical variables. |
|  | Statistical Visualizations | Used boxplots and histograms to explore `int.rate`, `installment`, and `revol.util`. |
| **Model Training** | Decision Tree Classifier | Trained a Decision Tree model to understand feature-based decision splits. |
|  | Random Forest Classifier | Implemented a Random Forest ensemble to improve accuracy and reduce overfitting. |
|  | Hyperparameter Tuning | Used `GridSearchCV` to find optimal model parameters. |
| **Model Evaluation** | Classification Metrics | Evaluated models using accuracy, precision, recall, and F1-score. |
|  | Confusion Matrix | Analyzed false positives and false negatives using confusion matrix. |
|  | Feature Importance | Identified key features influencing loan repayment predictions. |

## 📊 Visualizations

| Visualization | Description |
|---------------|------------|
| ![Credit Policy vs FICO](https://github.com/aashishh1/Decision-Trees-and-Random-Forest-Project/blob/main/Decision%20tress%20and%20random%20forest%20png/Histogram%20of%20two%20fico%20for%20each%20credit.policy.png) | Histogram comparing **FICO score distributions** based on `credit.policy` outcome. |
| ![Not Fully Paid vs FICO](https://github.com/aashishh1/Decision-Trees-and-Random-Forest-Project/blob/main/Decision%20tress%20and%20random%20forest%20png/histogram%20for%20two%20fico%20for%20not.fullly.paid.png) | Histogram showing **FICO score distributions** for loans that were fully paid vs not fully paid. |
| ![Loan Purpose Countplot](https://github.com/aashishh1/Decision-Trees-and-Random-Forest-Project/blob/main/Decision%20tress%20and%20random%20forest%20png/countplot%20for%20counts%20of%20loan%20by%20purpose%2C%20with%20hue%20defined%20by%20not.fully.paid.png) | Countplot displaying loan counts by **purpose**, with color hue based on `not.fully.paid`. |
| ![FICO vs Interest Rate](https://github.com/aashishh1/Decision-Trees-and-Random-Forest-Project/blob/main/Decision%20tress%20and%20random%20forest%20png/jointplot%20for%20fico%20rate%20and%20interest%20rate.png) | Jointplot illustrating the relationship between **FICO score** and **interest rate**. |
| ![Trend Comparison](https://github.com/aashishh1/Decision-Trees-and-Random-Forest-Project/blob/main/Decision%20tress%20and%20random%20forest%20png/lmplots%20for%20not.fully.paid%20and%20credit.policy.png) | Regression plots comparing trends across `credit.policy` and `not.fully.paid`. |



## 📌 Future Improvements
- **Advanced Hyperparameter Tuning**: Use RandomizedSearchCV for faster optimization.
- **Feature Engineering**: Create new features based on financial ratios for better predictions.
- **Comparison with Other Models**: Implement SVM, XGBoost, and Neural Networks for benchmarking.
- **Deployment**: Convert the model into a Flask API for real-world usability.
