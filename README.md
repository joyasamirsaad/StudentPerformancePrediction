# Student Performance Prediction

> Machine learning model to predict student math scores based on demographic and educational factors

# Project Overview

This AI Bootcamp final project develops a machine learning solution to predict student mathematics performance. Using a dataset of 1,000 student records, with Linear Regression.

# Key Features
- Predicts math scores based on 7 input features
- Comprehensive data analysis and visualization
- Educational insights for stakeholders

# Dataset

Source: [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

| Feature | Type | Description |
|---------|------|-------------|
| Gender | Categorical | Male/Female |
| Race/Ethnicity | Categorical | Group A-E |
| Parental Education | Categorical | Education level |
| Lunch | Categorical | Standard/Free-Reduced |
| Test Preparation | Categorical | Completed/None |
| Reading Score | Numerical | 0-100 |
| Writing Score | Numerical | 0-100 |
| Math Score | Target | 0-100 |

# Key Insights

- Reading & Writing scores are strongest predictors of math performance
- Standard lunch students outperform free/reduced lunch by 10-15 points
- Test preparation provides consistent 5-8 point improvement
- Female students perform better overall, males have slight math advantage
- Strong subject correlations (0.8+) across all test scores

# Clone repository
git clone https://github.com/joyasamirsaad/StudentPerformancePrediction.git
cd StudentPerformancePrediction

# Install dependencies
pip install -r requirements.txt

# Run analysis
jupyter notebook
```

# Project Structure

StudentPerformancePrediction/
├── 📊 data/Students.csv           # Dataset
├── 📓 notebook/project.ipynb      # Main analysis notebook
├── 📋 reports/                    # Project documentation
├── 🎥 demo/                       # Demo materials
├── 📄 requirements.txt            # Dependencies
└── 📖 README.md                   # This file


# Technologies Used

- Python - Core programming
- Pandas & NumPy - Data processing
- Scikit-learn - Machine learning
- Matplotlib & Seaborn - Visualization
- XGBoost & CatBoost - Advanced algorithms
- Jupyter Notebook - Development environment

# Usage Example

# Load and preprocess data
df = pd.read_csv('Students.csv')
X = df.drop('math_score', axis=1)
y = df['math_score']

# Train model
model = LinearRegression()
model.fit(X_processed, y)

# Make prediction
prediction = model.predict(new_student_data)
print(f"Predicted Math Score: {prediction[0]:.1f}")


# Business Impact

- Early intervention for at-risk students
- Personalized learning recommendations  
- Data-driven policy decisions
- Educational equity insights

# MLOps Lifecycle

Problem Definition  
Data Collection & Cleaning  
Exploratory Data Analysis  
Model Building & Training  
Evaluation & Tuning  
Documentation & Reporting  

# Authors

Nicolas Abou Chdid
Joya Saad
- Project: AI Bootcamp Final Project
- Date: June 2025

AI Bootcamp Final Project - Student Performance Prediction using Machine Learning # StudentPerformancePrediction
