# 🏥 Blood Bank Data Science Project

A complete end-to-end Data Science project for analyzing blood bank distribution across India using Python, Machine Learning, and interactive dashboards.

## 🎯 Features

- **Data Cleaning**: Automated data cleaning and standardization
- **EDA**: Comprehensive exploratory data analysis with visualizations
- **ML Clustering**: KMeans clustering to identify geographic patterns
- **Interactive Dashboard**: Gradio-powered web interface
- **Insights Generation**: Automated insights and recommendations

## 📁 Project Structure
```
blood-bank-project/
├── app.py                  # Gradio dashboard
├── eda.py                  # EDA analysis
├── model.py                # ML clustering
├── utils.py                # Data cleaning utilities
├── requirements.txt        # Dependencies
├── README.md              # Documentation
└── data/
    ├── blood_banks.csv            # Raw dataset
    ├── cleaned_blood_banks.csv    # Cleaned dataset
    └── clustered_blood_banks.csv  # Clustered dataset
```

## 🚀 Quick Start

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Prepare Your Data

Place your `blood_banks.csv` file in the `data/` folder with these columns:
- name
- address
- city
- state
- pincode
- contact
- email
- website
- latitude
- longitude

### 3. Run Data Cleaning
```bash
python utils.py
```

### 4. Run EDA
```bash
python eda.py
```

### 5. Run ML Clustering
```bash
python model.py
```

### 6. Launch Dashboard
```bash
python app.py
```

The dashboard will open in your browser at `http://localhost:7860`

## 📊 Dashboard Features

### Tab 1: Upload & Process
- Upload CSV file
- Automatic data cleaning
- Summary statistics

### Tab 2: Overview
- State-wise distribution charts
- City-wise distribution charts

 ### Tab 3: Geographic Visualization

Interactive map of blood bank locations
State-wise color coding

 ### Tab 4: ML Clustering

KMeans clustering (k=5)
Cluster visualization
Download clustered dataset

### Tab 5: Dataset Viewer

Filter by state/city
Search functionality
View cleaned data

🛠️ Technologies Used

Python 3.8+
pandas: Data manipulation
NumPy: Numerical computing
Matplotlib & Seaborn: Static visualizations
Plotly: Interactive visualizations
scikit-learn: Machine learning
Gradio: Web dashboard

📈 Analysis Outputs
The project generates:

Cleaned CSV datasets
EDA visualizations (saved in plots/)
Cluster analysis results
Automated insights report

🎓 Key Insights

Identifies states/cities with high blood bank density
Detects underserved regions
Provides geographic clustering for resource allocation
Generates data-driven recommendations
