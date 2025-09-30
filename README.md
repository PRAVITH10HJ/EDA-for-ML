# EDA-for-ML: Exploratory Data Analysis on Flipkart Drone Dataset

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PRAVITH10HJ/EDA-for-ML/blob/main/EDA_for_ML.ipynb)

## 📖 Overview

This project performs comprehensive **Exploratory Data Analysis (EDA)** on the Flipkart Drone dataset to prepare the data for machine learning applications. The analysis includes data cleaning, outlier detection and treatment, missing value imputation, feature engineering, and data preprocessing techniques.

## 📊 Dataset

The dataset contains information about drones sold on Flipkart with the following features:

- **Name**: Drone model name
- **Type**: Category of drone (Mini Drone, Professional Drone, etc.)
- **Control Range**: Maximum control range in meters
- **Battery Type**: Type of battery used (Lithium Battery, AA Battery, AA Rechargeable Battery)
- **Weight**: Weight of the drone in grams
- **Price**: Current selling price
- **Actual Price**: Original price before discount
- **Discount (%)**: Percentage discount offered

**Dataset Statistics:**
- Total Records: 821 drones
- Features: 8 columns

## 🔍 Analysis Performed

### 1. **Data Exploration**
   - Initial data inspection with `head()`, `info()`, and `describe()`
   - Shape and structure analysis
   - Data type verification

### 2. **Data Cleaning**
   - **Duplicate Removal**: Identified and removed duplicate entries
   - **Missing Value Treatment**: Handled null values using median imputation for numerical features with outliers

### 3. **Outlier Detection & Treatment**
   - Used **IQR (Interquartile Range) method** for outlier detection
   - Applied outlier capping to:
     - Control Range
     - Weight
     - Price
     - Actual Price
     - Discount (%)
   - Visualized outliers using box plots before and after treatment

### 4. **Statistical Analysis**
   - **Univariate Analysis**: Distribution plots for each feature
   - **Bivariate Analysis**: 
     - Pair plots to understand relationships between features
     - Correlation heatmap to identify feature correlations

### 5. **Data Preprocessing**
   - **Normalization and Scaling**: Applied StandardScaler to numerical features
     - Control Range
     - Weight
     - Price
     - Actual Price
     - Discount (%)
   - **Encoding**: One-Hot Encoding for categorical features
     - Name
     - Type
     - Battery Type

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries:**
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computing
  - `matplotlib` - Data visualization
  - `seaborn` - Statistical data visualization
  - `scikit-learn` - Machine learning preprocessing tools

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/PRAVITH10HJ/EDA-for-ML.git
cd EDA-for-ML
```

2. Open the Jupyter notebook:
```bash
jupyter notebook EDA_for_ML.ipynb
```

Or open directly in Google Colab using the badge at the top of this README.

### Usage

1. Ensure the `flipkart_drone.csv` file is in the same directory as the notebook
2. Run the cells sequentially to reproduce the analysis
3. Modify the code as needed for your own analysis

## 📁 Project Structure

```
EDA-for-ML/
│
├── EDA_for_ML.ipynb          # Main Jupyter notebook with EDA
├── flipkart_drone.csv        # Dataset file
└── README.md                 # Project documentation
```

## 📈 Key Insights

The EDA process revealed:
- Distribution patterns of drone prices and specifications
- Correlation between features (e.g., price vs. control range)
- Common battery types and drone categories
- Discount patterns across different drone types

## 🎯 Future Scope

- Build predictive models for drone price estimation
- Classification of drone types based on features
- Recommendation system for drone selection
- Additional feature engineering for improved model performance

## 👤 Author

**PRAVITH10HJ**

## 📝 License

This project is open source and available for educational purposes.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

---

**Note**: This project is part of a machine learning workflow where EDA is the crucial first step before model development.