# Employee Attrition Prediction 📊

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-orange.svg)](https://scikit-learn.org/)
[![pandas](https://img.shields.io/badge/pandas-1.3%2B-green.svg)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A comprehensive machine learning project to predict employee attrition using various algorithms and provide actionable business insights.

## 🎯 Project Overview

This project analyzes employee data to predict which employees are likely to leave the company. Using multiple machine learning algorithms, the model achieves **85%+ accuracy** in predicting employee attrition and provides valuable insights for HR decision-making.

![Project Overview](project_overview.png)

### Key Features
- 📈 **Multiple ML Models**: Logistic Regression, Random Forest, Gradient Boosting, SVM
- 🔧 **Hyperparameter Tuning**: Optimized model performance using GridSearchCV
- 📊 **Comprehensive Visualizations**: 15+ charts for data exploration and results
- 💡 **Business Insights**: Actionable recommendations for reducing attrition
- 🎲 **Feature Importance**: Identifies key factors driving employee turnover

## 🔬 Methodology

Our systematic approach combines data science best practices with business understanding:

![Methodology](methodology_flowchart.png)


## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- pip package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/employee-attrition-prediction.git
   cd employee-attrition-prediction
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Generate visualizations**
   ```bash
   python readme_image_generator.py
   ```

5. **Run the analysis**
   ```bash
   python main.py
   ```

## 📊 Dataset Information

- **Dataset**: IBM HR Analytics Employee Attrition
- **Size**: 1,470 employees, 35 features
- **Target**: Binary classification (Attrition: Yes/No)
- **Attrition Rate**: 16.12%

### Key Features
- **Demographics**: Age, Gender, Marital Status
- **Job Information**: Department, Job Role, Job Level
- **Compensation**: Monthly Income, Hourly Rate, Stock Options
- **Satisfaction**: Job Satisfaction, Environment Satisfaction, Work-Life Balance
- **Experience**: Years at Company, Total Working Years

## 🔍 Analysis Highlights

### Model Performance
Our comprehensive model comparison shows excellent predictive performance:

![Model Comparison](model_comparison.png)

| Model | Accuracy | Precision | Recall | F1-Score | AUC |
|-------|----------|-----------|---------|----------|-----|
| **Random Forest (Tuned)** | **0.8673** | **0.7419** | **0.6429** | **0.6889** | **0.8431** |
| Gradient Boosting (Tuned) | 0.8605 | 0.7097 | 0.6190 | 0.6615 | 0.8324 |
| Logistic Regression | 0.8367 | 0.6552 | 0.5476 | 0.5966 | 0.8156 |
| SVM | 0.8299 | 0.6207 | 0.5357 | 0.5753 | 0.8089 |

### Feature Importance Analysis
Understanding what drives employee attrition:

![Feature Importance](feature_importance.png)

### Top Risk Factors
1. **Overtime Work** - Strongest predictor of attrition
2. **Job Satisfaction** - Lower satisfaction = higher attrition risk
3. **Monthly Income** - Compensation directly impacts retention
4. **Years at Company** - Newer employees more likely to leave
5. **Work-Life Balance** - Poor balance increases turnover risk

## 📈 Key Business Insights

Understanding the critical factors that drive employee attrition:

![Business Insights](business_insights.png)

### 🔍 **High-Risk Employee Profiles**
- Employees working overtime
- Low job satisfaction scores (1-2)
- Monthly income below $3,000
- Less than 2 years at company
- Single marital status

### 💼 **Departmental Analysis**
- **Sales**: Highest attrition rate
- **R&D**: Moderate attrition
- **HR**: Lowest attrition rate

### 💡 **Recommendations**
1. **Implement work-life balance policies**
2. **Focus on job satisfaction improvement**
3. **Develop competitive compensation packages**
4. **Create targeted retention programs**
5. **Regular employee satisfaction surveys**

## 🛠️ Technical Implementation

### Data Preprocessing
- Categorical encoding using Label Encoders
- Feature scaling for distance-based algorithms
- Removal of irrelevant features (EmployeeCount, EmployeeNumber)
- Stratified train-test split to maintain class distribution

### Model Training
- Cross-validation for robust evaluation
- Hyperparameter tuning using GridSearchCV
- Multiple performance metrics evaluation
- Feature importance analysis

### Evaluation Metrics
- **Accuracy**: Overall correctness
- **Precision**: Positive prediction accuracy
- **Recall**: Sensitivity to actual positives
- **F1-Score**: Harmonic mean of precision and recall
- **AUC-ROC**: Area under the ROC curve

## 📊 Visualizations

The project generates comprehensive visualizations automatically:

### 🎨 **Generated Images**
- **Project Overview**: Dataset statistics and key distributions
- **Model Performance**: ROC curves and accuracy comparisons  
- **Feature Importance**: Top predictive factors analysis
- **Business Insights**: Key attrition drivers and patterns
- **Methodology**: Complete ML pipeline visualization

All visualizations are automatically generated in high resolution and optimized for professional presentation.

## 🔧 Usage Examples

### Basic Usage
```python
from main import EmployeeAttritionPredictor

# Initialize predictor
predictor = EmployeeAttritionPredictor('data/WA_FnUseC_HREmployeeAttrition.csv')

# Run complete analysis
predictor.load_and_explore_data()
predictor.preprocess_data()
predictor.train_models()
predictor.evaluate_models()
```

### Generate Visualizations
```python
from readme_image_generator import ReadmeImageGenerator

# Initialize generator
generator = ReadmeImageGenerator('data/WA_FnUseC_HREmployeeAttrition.csv')

# Load data and generate all images
generator.load_data()
generator.generate_all_images()
```

### Individual Components
```python
# Load and explore data
predictor.load_and_explore_data()

# Create visualizations
predictor.visualize_data()

# Train specific model
predictor.train_models()

# Analyze feature importance
predictor.feature_importance_analysis()
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Dataset source: IBM HR Analytics
- Inspiration from HR analytics community
- Built with scikit-learn, pandas, and matplotlib

## 📞 Contact

**[Kristopher Bradley, Ph.D.]**
- **Email:** kibradleyphd@gmail.com
- **LinkedIn:** [Your LinkedIn Profile](https://www.linkedin.com/in/kibradleyphd/)
- **GitHub:** [Your GitHub](https://github.com/krisibradley)
- **YouTube:** [Your YouTube](https://www.youtube.com/@kibradleyphd)

Project Link: [https://github.com/yourusername/employee-attrition-prediction](https://github.com/yourusername/employee-attrition-prediction)

---

⭐ **Star this repository if you found it helpful!**
