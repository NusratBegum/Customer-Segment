# 📊 E-Commerce Customer Segmentation & Analytics

A comprehensive data science project that performs end-to-end analysis on e-commerce transaction data, including customer segmentation, sales forecasting, and predictive modeling.

## 🎯 Project Overview

This project demonstrates a complete data science workflow using real-world e-commerce data from a UK-based online retailer. It includes data cleaning, exploratory data analysis (EDA), customer segmentation using RFM analysis and K-Means clustering, time series forecasting, and predictive modeling to identify high-value customers.

### Key Features

- ✅ **Data Cleaning & Preprocessing**: Handle missing values, outliers, and data quality issues
- ✅ **Exploratory Data Analysis**: Comprehensive visualization and statistical analysis
- ✅ **RFM Analysis**: Customer segmentation based on Recency, Frequency, and Monetary value
- ✅ **K-Means Clustering**: Identify distinct customer segments for targeted marketing
- ✅ **Time Series Forecasting**: Predict future sales trends using Exponential Smoothing
- ✅ **Predictive Modeling**: Machine learning models to identify high-value customers
- ✅ **Business Insights**: Actionable recommendations based on data analysis

## 📁 Dataset

- **Source**: UK-based online retail transactions
- **Period**: December 2010 - December 2011
- **Records**: 541,909 transactions
- **Features**: 
  - `InvoiceNo`: Invoice number
  - `StockCode`: Product code
  - `Description`: Product name
  - `Quantity`: Quantity purchased
  - `InvoiceDate`: Date and time of purchase
  - `UnitPrice`: Price per unit
  - `CustomerID`: Unique customer identifier
  - `Country`: Customer's country

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python libraries (see below)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/Customer-Segment.git
   cd Customer-Segment
   ```

2. **Install required packages**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
   ```

   Or create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook customer_seg.ipynb
   ```

### Required Libraries

```python
pandas          # Data manipulation
numpy           # Numerical computing
matplotlib      # Data visualization
seaborn         # Statistical visualization
scikit-learn    # Machine learning
statsmodels     # Time series analysis
```

## 📊 Project Structure

```
Customer-Segment/
│
├── customer_seg.ipynb              # Main analysis notebook
├── data.csv                        # Raw transaction data
├── cleaned_ecommerce_data.csv     # Cleaned dataset (generated)
├── customer_rfm_segments.csv      # RFM segmentation results (generated)
├── customer_features.csv          # Customer feature matrix (generated)
└── README.md                       # Project documentation
```

## 🔍 Analysis Sections

### 1. Data Ingestion & Cleaning
- Load and inspect the dataset
- Handle missing values and data quality issues
- Remove returns and cancellations
- Create derived features (TotalPrice)

### 2. Exploratory Data Analysis (EDA)
- Statistical summaries and distributions
- Time-based analysis (daily, weekly, monthly trends)
- Geographic analysis (revenue by country)
- Product analysis (top products, categories)
- Customer behavior patterns

### 3. Customer Segmentation (RFM Analysis)
- Calculate Recency, Frequency, and Monetary scores
- Assign RFM scores and segments
- Identify customer types:
  - 🏆 **VIP Champions**: High value, frequent buyers
  - 🌟 **Loyal Customers**: Regular purchasers
  - ⚠️ **At-Risk**: Previously active, now declining
  - 😴 **Hibernating**: Inactive customers

### 4. K-Means Clustering
- Standardize features
- Determine optimal number of clusters
- Visualize customer segments
- Analyze segment characteristics

### 5. Time Series Forecasting
- Aggregate sales by month
- Apply Exponential Smoothing
- Generate 6-month revenue forecast
- Visualize trends and predictions

### 6. Predictive Modeling
- Build customer feature matrix
- Train multiple models:
  - Logistic Regression
  - Random Forest Classifier
  - Gradient Boosting Classifier
- Evaluate model performance (accuracy, precision, recall, ROC AUC)
- Feature importance analysis

### 7. Executive Dashboard & Insights
- Key Performance Indicators (KPIs)
- Visual summary of findings
- Strategic recommendations

## 📈 Key Findings

### Customer Base
- UK customers dominate revenue (~82% of total sales)
- Strong international presence in Germany, France, and Ireland
- 4 distinct customer segments identified

### Sales Patterns
- Peak sales on Thursday; lowest on weekends
- Most purchases occur between 10 AM - 3 PM (business hours)
- Strong Q4 seasonality due to holiday shopping

### Customer Value
- Top 25% of customers contribute the majority of revenue
- VIP Champions segment has the highest monetary value
- At-risk customers need immediate re-engagement strategies

### Model Performance
- Random Forest achieves the best predictive performance
- Key predictors: Order frequency, recency, and product variety

## 💡 Business Recommendations

### Retention Strategy
- ✅ Implement VIP loyalty program for Champions segment
- ✅ Launch win-back campaigns for At-Risk customers
- ✅ Personalize offers based on purchase history

### Growth Strategy
- ✅ Expand marketing in high-potential EU markets
- ✅ Optimize website for peak shopping hours (10 AM - 3 PM)
- ✅ Increase promotional campaigns on Thursdays

### Operational Improvements
- ✅ Focus inventory on top 10 revenue-generating products
- ✅ Implement predictive models for high-value customer targeting
- ✅ Use sales forecasts for inventory and staffing planning

## 🛠️ Technologies Used

- **Python 3.x**: Primary programming language
- **Pandas & NumPy**: Data manipulation and numerical computing
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-learn**: Machine learning (clustering, classification)
- **Statsmodels**: Time series analysis and forecasting
- **Jupyter Notebook**: Interactive development environment

## 📝 Usage

1. Open `customer_seg.ipynb` in Jupyter Notebook
2. Run cells sequentially from top to bottom
3. Review visualizations and insights
4. Exported files will be saved in the project directory:
   - `cleaned_ecommerce_data.csv`: Cleaned dataset
   - `customer_rfm_segments.csv`: Customer segments
   - `customer_features.csv`: Feature matrix for modeling

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source. Please check with the repository owner for specific licensing terms.

## 📧 Contact

For questions or feedback, please reach out to the repository owner.

---

*This project demonstrates end-to-end data science skills and is perfect for portfolio showcase and data science job applications.*
