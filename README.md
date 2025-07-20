# 🌍 Country Data Clustering Analysis

This notebook performs comprehensive clustering analysis on country socioeconomic data, applying K-Means, Hierarchical, and DBSCAN clustering algorithms with enhanced data preprocessing and evaluation methods to identify patterns and groupings among countries based on various development indicators.

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

- **Objective:** Perform comprehensive clustering analysis on country socioeconomic data to identify development patterns and groupings using multiple advanced algorithms
- **Challenge:** Handle outliers, normalize diverse socioeconomic indicators, and implement robust data preprocessing for meaningful clustering
- **Solution:** Apply comprehensive data preprocessing, multiple clustering algorithms, and advanced evaluation methods
- **Features Used:** Child mortality, exports, health spending, imports, income, inflation, life expectancy, total fertility, GDP per capita
- **Target:** Unsupervised learning to discover natural groupings among countries using multiple clustering approaches with enhanced validation

---

## 🧪 Methods

- **Models Used:**
  - 🎯 K-Means Clustering (with optimal k selection)
  - 🌳 Hierarchical Clustering (with dendrogram visualization)
  - 📦 DBSCAN Clustering (with eps parameter optimization)
  - 📊 Principal Component Analysis (PCA)

- **Enhanced Data Preprocessing:**
  - 🔍 Comprehensive outlier detection and removal using IQR method
  - 📋 Handling unique and duplicate records
  - 🔧 Advanced feature engineering and data preparation
  - 📊 Data visualization with distribution plots and correlation heatmaps
  - 🔧 StandardScaler for feature normalization
  - 📈 Silhouette score evaluation for clustering quality
  - 🎨 PCA for dimensionality reduction and visualization
  - 📋 Duplicate removal and data validation
  - 📊 Box plots and histograms for distribution analysis
  - 🌳 Dendrogram visualization for hierarchical clustering
  - 📦 DBSCAN parameter tuning with eps optimization (0.3-1.0)
  - 🔄 Multi-algorithm comparison and performance analysis
  - 🧮 Mathematical calculations for optimal parameter selection

---

## 📈 Results

### **Comprehensive Clustering Performance Comparison**
| Model | Silhouette Score | Performance | Optimal Parameters | Clusters |
|-------|------------------|-------------|-------------------|----------|
| 🎯 K-Means | **0.4240** | **Best Performance** | k=2 | 2 |
| 🌳 Hierarchical | 0.4131 | Excellent Performance | k=2 | 2 |
| 📦 DBSCAN | 0.2626 | Good Performance | eps=0.5, min_samples=5 | 3 |

### **DBSCAN Parameter Optimization Results**
| Eps Value | Clusters | Silhouette Score | Status |
|-----------|----------|------------------|--------|
| 0.3 | 4 | -0.3266 | Poor |
| 0.4 | 10 | -0.0420 | Poor |
| 0.5 | 3 | **0.2626** | **Optimal** |
| 0.6 | 3 | 0.1726 | Good |
| 0.7+ | 1 | N/A | Single Cluster |

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
- **K-Means Superiority**: K-Means achieved the best silhouette score (0.4240) with optimal k=2
- **Enhanced Data Preprocessing**: Comprehensive outlier removal and duplicate handling significantly improved clustering quality
- **DBSCAN Optimization**: Successfully implemented DBSCAN with parameter tuning, finding optimal eps=0.5
- **Consistent Performance**: Both K-Means and Hierarchical clustering identified 2 optimal clusters
- **Outlier Impact**: Significant outlier removal improved clustering quality and interpretability
- **Economic Clustering**: Countries naturally grouped by income levels and development status
- **Feature Relationships**: Strong correlations between health spending, income, and life expectancy
- **Development Patterns**: Clear separation between developed and developing nations
- **Data Quality**: Enhanced preprocessing improved model performance and reliability
- **Algorithm Comparison**: Multi-algorithm approach provides robust clustering validation
- **Parameter Optimization**: Systematic parameter tuning for DBSCAN improved clustering results

---

## 🧾 Project Details

**🔧 Enhanced Data Preprocessing:**
- Comprehensive outlier detection using IQR method
- Handling unique and duplicate records
- Advanced feature engineering and data preparation
- Feature scaling and normalization
- Duplicate removal and data validation
- Missing value analysis

**📊 Advanced Exploratory Data Analysis:**
- Distribution analysis for all features
- Correlation heatmap visualization
- Box plots for outlier identification
- Statistical summary analysis
- Enhanced data visualization techniques

**🎯 Multi-Algorithm Clustering Implementation:**
- K-Means clustering with optimal k selection (k=2)
- Hierarchical clustering with dendrogram visualization
- DBSCAN clustering with comprehensive eps parameter tuning
- PCA for dimensionality reduction
- Silhouette score evaluation for all algorithms
- Parameter optimization for each algorithm

**📈 Enhanced Visualization & Results:**
- PCA-based cluster visualization for all algorithms
- Comprehensive performance comparison between algorithms
- DBSCAN parameter optimization results visualization
- Detailed statistical analysis
- Multi-algorithm clustering comparison
- Silhouette score analysis for different parameters

**📋 Enhanced Notebook Structure:**
- Data Loading & Initial Exploration
- Enhanced Data Preprocessing
  - Handling Unique and Duplicate Records
  - Comprehensive Outlier Detection & Removal
- Advanced Exploratory Data Analysis
- Feature Engineering & Data Preparation
- Multi-Algorithm Clustering Implementation
  - K-Means Clustering with Optimal k Selection
  - Hierarchical Clustering with Dendrogram
  - DBSCAN Clustering with Parameter Tuning
- Comprehensive Results Comparison & Visualization
- Algorithm Performance Analysis with Silhouette Scores

---

## 🪪 License

This project is for educational and non-commercial use only.  
Dataset source: [Kaggle Country Data for Unsupervised Learning](https://www.kaggle.com/datasets/rohan0301/unsupervised-learning-on-country-data) 