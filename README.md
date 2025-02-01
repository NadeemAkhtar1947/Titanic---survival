# 🚢 Titanic Survival Prediction

## 📝 Overview
This project predicts **Titanic passenger survival** using **Machine Learning models**. The dataset includes passenger details like **age, gender, fare, and ticket class**, and the models classify whether a passenger survived or not.

## 📂 Dataset
- **📌 Source:** Titanic Dataset from Kaggle
- **📑 Files:**
  - `train.csv`: Training dataset with labels (`Survived` column).
  - `test.csv`: Test dataset for prediction.
  - `gender_submission.csv`: Sample submission file.
- **📊 Data Preprocessing:**
  - Handled missing values in **Age, Embarked, and Cabin**.
  - Removed unnecessary columns (`Name`, `Ticket`, `Cabin`, `Embarked`).
  - Encoded categorical variables (**Sex**) using **Label Encoding**.
  - Scaled numerical features for better performance.

## 🤖 Machine Learning Models
### 🌳 **Decision Tree Classifier**
- Trained on **Pclass, Sex, SibSp, Parch, Fare**.
- Achieved **92.26% accuracy** on the training dataset.

### 🌲 **Random Forest Classifier**
- Used **150 estimators** with **max depth = 5**.
- Achieved **81.59% accuracy**.

## 🚀 Implementation Steps
1. **Load and Preprocess Data**
2. **Feature Engineering:** Encode categorical variables, scale numerical features.
3. **Train Decision Tree Model**
4. **Train Random Forest Model**
5. **Generate Predictions and Save Submission File**
   ```python
   output = pd.DataFrame({'PassengerId': test_df.PassengerId, 'Survived': predictions})
   output.to_csv('submission.csv', index=False)
   print("Your submission was successfully saved!")
   ```

## 🛠️ Installation & Usage
### **📌 Requirements**
Ensure you have the following Python libraries installed:
```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

### **▶️ Running the Code**
```bash
python titanic_survival.py
```

## 🎯 Future Enhancements
- Implement **Deep Learning models** (e.g., Neural Networks).
- Use **Feature Engineering** to extract more meaningful insights.
- Improve hyperparameter tuning using **GridSearchCV**.

## 📬 Contact & Support
Connect with me for feedback or contributions:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nadeem-akhtar-/) | [![GitHub](https://img.shields.io/badge/GitHub-333?style=for-the-badge&logo=github&logoColor=white)](https://github.com/NadeemAkhtar1947) | [![Kaggle](https://img.shields.io/badge/Kaggle-00A65A?style=for-the-badge&logo=Kaggle&logoColor=white)](https://www.kaggle.com/mdnadeemakhtar/code) | [![Portfolio](https://img.shields.io/badge/Portfolio-FF5733?style=for-the-badge&logo=Google-chrome&logoColor=white)](https://nsde.netlify.app/)

🚀 **Developed by Nadeem Akhtar** | 📅 **Copyright © 2025**

