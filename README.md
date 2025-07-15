# 🌍 Country Data Clustering Analysis

This notebook performs comprehensive clustering analysis on country socioeconomic data, applying K-Means and Hierarchical clustering algorithms to identify patterns and groupings among countries based on various development indicators.

---

## 📚 Table of Contents

- [💻 Installation](#-installation)
- [🎯 Project Goals](#-project-goals)
- [🧪 Methods](#-methods)
- [📈 Results](#-results)
- [🔍 Key Insights](#-key-insights)
- [🧾 Project Details](#-project-details)
- [🪪 License](#-license)

---

## 💻 Installation

- **Requirements:** Python 3.8+, Jupyter Notebook

```bash
# Clone the repository
git clone https://github.com/alhussienhazem/country-clustering-analysis.git

# Navigate to the project folder
cd country-clustering-analysis

# (optional) create a virtual environment
python -m venv venv
source venv/bin/activate  # on Linux/Mac
venv\Scripts\activate     # on Windows

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook
```

---

## 🎯 Project Goals

- **Objective:** Perform clustering analysis on country socioeconomic data to identify development patterns and groupings
- **Challenge:** Handle outliers and normalize diverse socioeconomic indicators for meaningful clustering
- **Solution:** Apply comprehensive data preprocessing and multiple clustering algorithms
- **Features Used:** Child mortality, exports, health spending, imports, income, inflation, life expectancy, total fertility, GDP per capita
- **Target:** Unsupervised learning to discover natural groupings among countries

---

## 🧪 Methods

- **Models Used:**
  - 🎯 K-Means Clustering
  - 🌳 Hierarchical Clustering
  - 📊 Principal Component Analysis (PCA)

- **Techniques Applied:**
  - 🔍 Comprehensive outlier detection and removal using IQR method
  - 📊 Data visualization with distribution plots and correlation heatmaps
  - 🔧 StandardScaler for feature normalization
  - 📈 Silhouette score evaluation for clustering quality
  - 🎨 PCA for dimensionality reduction and visualization
  - 📋 Duplicate removal and data validation
  - 📊 Box plots and histograms for distribution analysis

---

## 📈 Results

### **Clustering Performance**
| Model | Silhouette Score | Performance |
|-------|------------------|-------------|
| 🎯 K-Means | 0.2783 | **Best Performance** |
| 🌳 Hierarchical | 0.2657 | Good Performance |

---

### **Key Features Analyzed**
| Feature | Description | Impact |
|---------|-------------|--------|
| 👶 Child Mortality | Deaths per 1000 children | High correlation with development |
| 💰 Income | Per capita income | Strong clustering factor |
| 🏥 Health | Healthcare spending % | Development indicator |
| 📈 GDP | GDP per capita | Economic development measure |
| 👴 Life Expectancy | Average life span | Quality of life indicator |
| 📊 Exports/Imports | Trade balance | Economic activity |
| 💸 Inflation | Price stability | Economic health |

---

### **🔍 Key Insights**
- **K-Means Superiority**: K-Means achieved better silhouette score (0.2783) compared to Hierarchical clustering
- **Outlier Impact**: Significant outlier removal improved clustering quality and interpretability
- **Economic Clustering**: Countries naturally grouped by income levels and development status
- **Feature Relationships**: Strong correlations between health spending, income, and life expectancy
- **Development Patterns**: Clear separation between developed and developing nations
- **Data Quality**: Comprehensive preprocessing improved model performance and reliability

---

## 🧾 Project Details

**🔧 Enhanced Data Preprocessing:**
- Comprehensive outlier detection using IQR method
- Feature scaling and normalization
- Duplicate removal and data validation
- Missing value analysis

**📊 Exploratory Data Analysis:**
- Distribution analysis for all features
- Correlation heatmap visualization
- Box plots for outlier identification
- Statistical summary analysis

**🎯 Clustering Implementation:**
- K-Means clustering with optimal parameters
- Hierarchical clustering for comparison
- PCA for dimensionality reduction
- Silhouette score evaluation

**📈 Visualization & Results:**
- PCA-based cluster visualization
- Performance comparison between algorithms
- Detailed statistical analysis
- Comprehensive reporting

**📋 Notebook Structure:**
- Data Loading & Initial Exploration
- Outlier Detection & Removal
- Exploratory Data Analysis
- Feature Engineering & Scaling
- Clustering Implementation
- Results Comparison & Visualization

---

## 🪪 License

This project is for educational and non-commercial use only.  
Dataset source: [Kaggle Country Data for Unsupervised Learning](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data) 