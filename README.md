# Student Performance Prediction  

This project predicts students' academic performance based on demographic and educational features. It employs various regression algorithms, with **CatBoost Regressor** achieving the best results. The project is structured as a machine learning pipeline with modular components for data ingestion, transformation, model training, and deployment.  

---

## 🚀 **Project Overview**  

### 📂 **Dataset**  
The dataset contains the following features:  
- **Gender** – Student’s gender.  
- **Ethnicity** – Student’s ethnicity.  
- **Parental Education Level** – Highest education level attained by parents.  
- **Lunch Type** – Type of lunch (standard/reduced).  
- **Test Preparation Status** – Whether the student completed test preparation.  
- **Scores** – Test scores in math, reading, and writing.  

### 🎯 **Objective**  
To predict students' test scores using machine learning regression techniques.  

### 🏆 **Best Model**  
- **CatBoost Regressor** achieved the highest R² score of **87%**.  

---

## 🔑 **Key Features**  
✅ **Pipeline Implementation:**  
- Modular components for ingestion, transformation, and training ensure scalability and reusability.  

✅ **Best Model:**  
- CatBoost Regressor with an R² score of **87%**.  

✅ **Web Interface:**  
- Flask-based web app for user interaction.  

✅ **CI/CD Integration:**  
- Automated workflows using **GitHub Actions**.  

---

## 📁 **Project Structure**  
```plaintext
├── .github/workflows/  
│   └── main_studentperformancepred.yml  # CI/CD workflow configuration  
├── artifacts/  
│   ├── data.csv                         # Full dataset  
│   ├── model.pkl                        # Saved CatBoost model  
│   ├── preprocessor.pkl                 # Saved preprocessor  
│   ├── test.csv                         # Testing dataset  
│   ├── train.csv                        # Training dataset  
├── catboost_info/                       # CatBoost training logs  
├── notebook/  
│   └── eda_and_model_training.ipynb     # Jupyter notebook for EDA and training  
├── src/  
│   ├── components/                      # Core components  
│   │   ├── __init__.py  
│   │   ├── data_ingestion.py            # Data ingestion pipeline  
│   │   ├── data_transformation.py       # Data preprocessing and transformation  
│   │   └── model_trainer.py             # Model training pipeline  
│   ├── pipeline/  
│   │   ├── __init__.py  
│   │   ├── predict_pipeline.py          # Prediction pipeline  
│   │   └── train_pipeline.py            # Training pipeline  
│   ├── __init__.py  
│   ├── exception.py                     # Custom exception handling  
│   ├── logger.py                        # Logging setup  
│   └── utils.py                         # Utility functions  
├── templates/                           # HTML templates for web interface  
│   ├── home.html  
│   └── index.html  
├── .gitignore                           # Git ignore file  
├── README.md                            # Project documentation  
├── app.py                               # Flask application for deployment  
├── requirements.txt                     # Python dependencies  
├── setup.py                             # Package setup file  

