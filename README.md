# Neural Network-Based Credit Risk Prediction Using MLP

A deep learning project for predicting loan defaults using Multi-Layer Perceptron (MLP) neural networks.

## 📋 Project Overview

This project implements a neural network-based system to predict whether a loan applicant will default on their loan. The model analyzes various financial and demographic features to provide accurate risk assessments, helping financial institutions make informed lending decisions.

### Student Information
- **Name**: Jitin Kumar Sengar
- **Roll Number**: 2501940073
- **Course**: Deep Learning Architectures and Techniques
- **Course Code**: ETMMDL274

## 🎯 Objectives

- Implement a Multi-Layer Perceptron (MLP) for binary classification
- Perform comprehensive data preprocessing and feature engineering
- Achieve high prediction accuracy for loan default detection
- Demonstrate understanding of deep learning fundamentals
- Apply neural networks to real-world financial data

## 📁 Project Structure

```
Deep-Learning-Assignment-1/
├── Data/
│   └── Loan_Default.csv          # Dataset containing loan application records
├── Notebook/
│   └── notebook.ipynb            # Main Jupyter notebook with complete implementation
├── Report/
│   └── (Project reports and documentation)
├── .gitattributes                # Git attributes configuration
├── .gitignore                    # Git ignore rules
└── README.md                     # This file
```

## 🔧 Technologies Used

- **Python 3.x**
- **TensorFlow/Keras** - Deep learning framework
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Scikit-learn** - Machine learning utilities (preprocessing, metrics)

## 📊 Dataset

The **Loan Default Dataset** contains information about loan applicants including:
- **Demographics**: Age, gender, region
- **Financial Information**: Income, credit score, loan amount, interest rate
- **Loan Details**: Loan type, loan-to-value ratio, employment length
- **Property Information**: Property value, property age
- **Target Variable**: Status (1 = Default, 0 = No Default)

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Deep-Learning-Assignment-1
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Open the Jupyter notebook:
```bash
jupyter notebook Notebook/notebook.ipynb
```

## 🔬 Methodology

### 1. Data Preprocessing
- **Data Loading**: Load the Loan Default dataset
- **Data Inspection**: Analyze structure, data types, and missing values
- **Feature Selection**: Remove irrelevant columns (ID)
- **Missing Value Handling**: 
  - Numerical features: Fill with median
  - Categorical features: Fill with mode
- **Encoding**: One-hot encode categorical variables
- **Feature Scaling**: Standardize features using StandardScaler

### 2. Model Architecture
```
Input Layer (49 features)
    ↓
Hidden Layer 1 (64 neurons, ReLU activation)
    ↓
Hidden Layer 2 (32 neurons, ReLU activation)
    ↓
Output Layer (1 neuron, Sigmoid activation)
```

### 3. Training Configuration
- **Loss Function**: Binary Cross-Entropy
- **Optimizer**: Adam
- **Metrics**: Accuracy
- **Epochs**: 20
- **Batch Size**: 32
- **Train-Test Split**: 80-20

### 4. Model Evaluation
- **Confusion Matrix**: Visualize prediction performance
- **Accuracy Score**: Overall correctness
- **Classification Report**: Precision, Recall, F1-Score
- **Training Curves**: Monitor learning progress

## 📈 Results

The model achieved exceptional performance:

| Metric | Score |
|--------|-------|
| **Accuracy** | ~99.85% |
| **Precision** | ~1.0 |
| **Recall** | ~1.0 |
| **F1-Score** | ~1.0 |

**Key Findings:**
- ✅ High accuracy with minimal overfitting
- ✅ Training and validation curves converge smoothly
- ✅ Model generalizes well to unseen data
- ✅ Balanced performance across all metrics

## 🎓 Key Learnings

1. **Data Quality Matters**: Proper preprocessing is crucial for model performance
2. **Feature Scaling**: Standardization significantly improves neural network training
3. **Architecture Design**: Two hidden layers provide sufficient capacity for this task
4. **Evaluation**: Multiple metrics give a comprehensive view of model performance
5. **Real-World Application**: Deep learning is highly effective for credit risk assessment

## 💼 Real-World Applications

This model can be used by financial institutions to:
- **Automate loan approval decisions** - Faster processing with consistent criteria
- **Reduce financial losses** - Identify high-risk applicants early
- **Improve risk management** - Data-driven lending strategies
- **Ensure fairness** - Reduce human bias in decision-making
- **Optimize operations** - Scale lending operations efficiently

## 📝 Future Enhancements

- [ ] Implement cross-validation for more robust evaluation
- [ ] Experiment with different architectures (deeper networks, different activation functions)
- [ ] Add dropout layers to further prevent overfitting
- [ ] Hyperparameter tuning using grid search or Bayesian optimization
- [ ] Test alternative models (Random Forest, XGBoost, ensemble methods)
- [ ] Feature importance analysis to understand key predictors
- [ ] Deploy model as a web service (Flask/FastAPI)
- [ ] Create interactive dashboard for predictions

## 🤝 Contributing

This is an academic project. However, suggestions and feedback are welcome:
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

This project is created for educational purposes as part of the Deep Learning course.

## 📧 Contact

**Jitin Kumar Sengar**
- Roll Number: 2501940073
- Course: Deep Learning Architectures and Techniques (ETMMDL274)

---

## 🙏 Acknowledgments

- Course instructors and teaching assistants
- Deep Learning community for resources and best practices
- TensorFlow/Keras documentation and tutorials
- Scikit-learn for excellent preprocessing tools

---
