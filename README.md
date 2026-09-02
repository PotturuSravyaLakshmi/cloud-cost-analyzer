# ☁️ Cloud Cost Analyzer

A Python-based **Cloud Cost Analyzer** that processes monthly cloud billing CSV files, combines them into a single dataset, analyzes cloud spending, identifies unused resources, and visualizes cost trends using **Pandas** and **Matplotlib**.

## 📌 Project Overview

Cloud Cost Analyzer helps analyze cloud billing data by combining multiple monthly billing files into one dataset. It provides insights into:

* Total cloud cost
* Cost by cloud service
* Monthly cost breakdown
* Unused resources
* Yearly/monthly spending trends
* Service-wise cost visualization

## 🚀 Features

* 📂 Reads multiple monthly cloud billing CSV files
* 🔗 Combines billing data into a single DataFrame
* 💰 Calculates total cloud cost
* 📊 Calculates cost by service
* 📅 Provides monthly cost breakdown
* ⚠️ Identifies unused resources based on zero usage hours
* 📈 Generates service-wise cost visualization
* 📉 Generates monthly cloud cost trend visualization

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **Matplotlib**

## 📁 Project Structure

```text
cloud-cost-analyzer/
│
├── cloud_cost_analyzer.py
├── cloud_billing_january.csv
├── cloud_billing_february.csv
├── cloud_billing_march.csv
├── cloud_billing_heavy_usage.csv
├── README.md
```

## 📊 Input Data

The project uses cloud billing CSV files following the naming pattern:

```text
cloud_billing_*.csv
```

The Python program automatically finds these files and combines them into a single dataset.

The billing data contains information such as:

* Date
* Service
* Resource
* Usage Hours
* Cost

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/cloud-cost-analyzer.git
```

### 2. Navigate to the project directory

```bash
cd cloud-cost-analyzer
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

## ▶️ How to Run

Run the following command:

```bash
python cloud_cost_analyzer.py
```

The program will:

1. Read all matching billing CSV files.
2. Combine the billing data.
3. Convert the date column into datetime format.
4. Calculate the total cloud cost.
5. Calculate service-wise costs.
6. Generate a monthly cost breakdown.
7. Identify resources with zero usage hours.
8. Display service-wise and monthly cost graphs.

## 📈 Visualizations

The project generates two visualizations:

### 1. Yearly Cloud Cost by Service

A bar chart showing the total cost associated with each cloud service.

### 2. Monthly Cloud Cost Trend

A line chart showing how cloud spending changes month by month.

## 🔍 Resource Optimization

The project identifies potentially unused resources by checking for resources where:

```text
UsageHours = 0
```

These resources can be reviewed to identify possible opportunities for cloud cost optimization.

## 🎯 Learning Outcomes

Through this project, I practiced:

* Python programming
* Pandas DataFrame operations
* Reading and combining CSV files
* Data cleaning and transformation
* GroupBy analysis
* Date/time data analysis
* Cloud cost analysis
* Data visualization using Matplotlib
* Basic Git and GitHub workflow

## 🔮 Future Improvements

* Add an interactive dashboard using Streamlit
* Add cloud provider support for AWS, Azure, and Google Cloud
* Add cost forecasting
* Detect underutilized resources
* Add automated cost optimization recommendations
* Export analysis results to Excel/PDF
* Add interactive filters and charts
