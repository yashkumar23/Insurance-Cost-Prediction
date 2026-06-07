# 🏥 Insurance Cost Prediction

## 📌 Project Overview & Task Objective

This repository contains a Jupyter Notebook (`insurance_cost_predictions.ipynb`) focused on predicting **medical insurance charges**.  
The primary objective is to build a **Linear Regression model** that can accurately estimate insurance costs based on personal and health-related features like **age**, **BMI**, and **smoking status**, using the `insurance.csv` dataset.

## 📊 Dataset Information

The dataset includes information about individuals and their insurance charges.

**Target variable**: `charges`  
**Key features**:
- `age`
- `sex`
- `bmi`
- `children`
- `smoker`
- `region`

Categorical features such as `sex`, `smoker`, and `region` were converted into numerical format using encoding techniques.

## 🧩 Features

- Data loading and initial inspection  
- Handling missing values (if any)  
- Encoding categorical variables  
- Exploratory Data Analysis (EDA)  
- Training a Linear Regression model  
- Evaluating model performance using MAE and MSE  

## ⚙️ Installation

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🔍 Approach
My approach to Insurance cost prediction involved the following steps:
1. **Library Import**: Imported essential libraries like `pandas`, `numpy`, `matplotlib`, `seaborn`, and `sklearn`  
2. **Data Loading**: Loaded the `insurance.csv` dataset into a DataFrame  
3. **Data Preparation**:  
   - Checked for and handled any missing values (none
     found in this dataset).
   - Encoded Categorical Variables: smoker and sex were
     mapped to numerical values, and region was converted using one-hot encoding
     ( pd.get_dummies ).
4. **Exploratory Data Analysis**:  
   - Analyzed feature distributions and their relationships with the charges target variable. This involved visualizing
     distributions and correlations.   
5. **Model Training & Evaluation**:  
   - Split data into training and test sets  
   - Trained `Linear Regression model` 
6. **Model Evaluation**:
   - Evaluated the trained model using metrics such as Mean Absolute Error (MAE) and Mean Squared Error (MSE)
     to assess its performance in predicting insurance charges.

## 💻 Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

## 📊 Visualizations

- Scatter plots of numerical features `smokers`,`bmi`,`charges`
  ![image](https://github.com/user-attachments/assets/33cd7e67-a2a9-49b6-9e5b-b7b7c5ba6d71)

  **Insights:**
  The above Graph shows:
  - For non-smokers, insurance charges increase slowly as BMI rises.
  - For smokers, the charges increase sharply, especially with high BMI.
  - It means overweight and smoking together greatly increase insurance costs.
    
- Scatter plots of numerical features `smokers`,`age` vs `charges`
  ![image](https://github.com/user-attachments/assets/a67b4d43-bd2b-4be2-a1cc-1716c42ff325)

  **Insights:**
  The above Graph shows:
  - As people get older, their insurance charges usually go higher.
  - This happens even more for people who smoke.
  - Older people are more likely to have health problems, so they cost more to insure.
    
- Box plot of  `smoker` vs `charges`
  ![image](https://github.com/user-attachments/assets/a4e60e27-99d7-47f9-83e9-7549d856d48b)

  **Insights:**
  The Above Graph shows:
  - Smokers pay much higher insurance charges than non-smokers.
  - On average, smokers' charges are more than double.
  - Smoking increases health risks, so insurers predict higher costs.

## 📈 Results and Insights

- **Feature Importance**: `smoker`, `BMI`, and `age` are strong predictors  
- **Smoker**: Has the most significant impact on charges  
- **Model Performance**:  
  - Linear Regression gave a reasonable fit  
  - MAE and RMSE provided average prediction error magnitudes
  - MAE: The model is usually off by about `$2,711` when predicting charges.
  - RMSE: The average error is around `$4,506`, and it gives more importance to bigger mistakes.
  - Smaller values mean the model is making more accurate predictions.
- **Visual Analysis**:
  - Clear relationships between smoking status and charges  
  - Box plots and scatter plots support insights  
  - Correlation heatmap helped detect feature relevance

## ▶️ Usage

```bash
# Clone the repository
git clone https://github.com/Shilpachhatani/Insurance-Cost-Prediction.git

# Navigate into the folder
cd Insurance-Cost-Prediction

# Run the notebook
jupyter notebook insurance_cost_predictions.ipynb
```

## 🤝 Contributing

Contributions are welcome!  
Please fork the repository, open an issue, or submit a pull request.

## 📬 Contact

- **GitHub**: `yashkumar23`
- **Email**: yashchhatani7@gmail.com 
