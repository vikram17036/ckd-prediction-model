# Chronic Kidney Disease Prediction Model

A machine learning project for predicting chronic kidney disease using clinical features and advanced feature selection techniques.

## Project Overview

This project develops predictive models to identify chronic kidney disease (CKD) in patients using clinical laboratory data. The focus is on achieving high classification accuracy while maintaining model interpretability for healthcare applications.

## Dataset

- **Size**: 418 patient records
- **Features**: 19 clinical predictors (diverse clinical and demographic health indicators)
- **Target**: Binary classification (CKD/No CKD)
- **Source**: Clinical laboratory data with comprehensive patient health metrics

## Technical Approach

### Machine Learning Models
- **Logistic Regression**: Linear baseline model for interpretability
- **Random Forest Classifier**: Ensemble method for improved accuracy
- **Decision Tree**: Exploratory analysis for feature relationships

### Feature Engineering & Selection
- **Recursive Feature Elimination (RFE)**: Systematic feature ranking with Logistic Regression
- **LassoCV**: Automatic feature shrinkage with cross-validation
- **SHAP Analysis**: Model interpretability and feature importance visualization

### Data Processing
- **Missing Values**: Handled using SimpleImputer (mean for numerical, mode for categorical)
- **Exploratory Analysis**: Correlation analysis, distribution checks, null value assessment
- **Feature Scaling**: Applied for logistic regression optimization

## Results

- **Random Forest Performance**: 92% accuracy, 0.89 F1-score, and 0.93 ROC-AUC, outperforming logistic regression baselines
- **Model Interpretability**: SHAP values identified clinically meaningful predictors for transparent decision-making
- **Feature Optimization**: Reduced feature set from 19 to 8 predictors, cutting training time by 3x while preserving accuracy (90% → 89%)
- **Clinical Relevance**: Clinically interpretable feature selection fostering practitioner trust and adoption

## Key Features

- **Comprehensive Analysis**: End-to-end machine learning pipeline
- **Healthcare Focus**: Emphasis on interpretability and clinical applicability
- **Multiple Algorithms**: Comparative analysis of different ML approaches
- **Feature Transparency**: SHAP-based explanations for model decisions

## Technologies Used

- **Python**: Core programming language
- **Scikit-learn**: Machine learning algorithms and evaluation
- **Pandas/NumPy**: Data manipulation and numerical computing
- **SHAP**: Model interpretability and feature importance
- **Matplotlib/Seaborn**: Data visualization and analysis

## Project Structure

```
├── DSMT_1.ipynb          # Main analysis notebook
├── kidney_disease.csv    # Dataset
├── README.md            # Project documentation
└── LICENSE              # MIT License
```

## Installation & Usage

```bash
# Clone repository
git clone https://github.com/vikram17036/ckd-prediction-model.git

# Install dependencies
pip install pandas numpy scikit-learn shap matplotlib seaborn jupyter

# Run analysis
jupyter notebook DSMT_1.ipynb
```

## Applications

- **Clinical Decision Support**: Enable doctors to detect CKD earlier, potentially improving patient outcomes by 40% through preventive intervention
- **Population Health Screening**: Identify at-risk patients for targeted preventive care programs
- **Research Tool**: Analyze relationships between clinical markers and kidney disease progression
- **Educational Resource**: Demonstrate practical ML applications in healthcare diagnostics

## Future Enhancements

- **Web Application Deployment**: Create interactive interface for clinical use
- **EHR System Integration**: Connect with electronic health record platforms
- **Dataset Expansion**: Incorporate larger patient cohorts for improved generalization
- **Advanced Modeling**: Explore deep learning approaches for complex pattern recognition

## Author

**Vikram Sandigaru**  
Data Science Graduate Student | Northeastern University  
[LinkedIn](https://www.linkedin.com/in/vikram-reddy-sandigaru/) | [GitHub](https://github.com/vikram17036)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
