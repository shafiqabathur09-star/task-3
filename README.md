Retail Sales Data Analysis & Cleaning
This project focuses on preprocessing, analyzing, and describing a synthetic retail sales dataset containing 1,000 transaction records. The analysis includes missing data handling, data type verification, descriptive statistics computation, and data visualization.

📊 Dataset Structure
The generated dataset contains 1,000 rows and 9 columns:

Column Name	Data Type	Description	Missing Values
Transaction_ID	int64	Unique transaction identifier	0
Date	datetime64[us]	Date of purchase (2025-01-01 to 2027-09-27)	0
Customer_Age	float64	Age of the customer	20 (Imputed)
Gender	str	Male / Female	0
Product_Category	str	Category (Electronics, Clothing, Home & Kitchen, Books, Beauty)	0
Product_ID	str	Product code (PROD_1 to PROD_20)	0
Quantity	int32	Units purchased per transaction (1 to 5)	0
Price_Per_Unit	float64	Unit price in USD ($10.00 – $500.00)	0
Total_Sales	float64	Total transaction amount (Quantity × Price_Per_Unit)	0
📈 Descriptive Statistics
Summary statistics computed across key numerical features:

Metric	Customer_Age	Quantity	Price_Per_Unit ($)	Total_Sales ($)
Mean	43.81	3.07	252.33	771.10
Median	44.00	3.00	252.99	627.16
Mode	44.00	5.00	36.35	205.16
Std Dev	14.85	1.40	141.57	590.34
Min	18.00	1.00	10.09	17.02
Max	69.00	5.00	498.49	2487.00
⚙️ Key Steps & Workflow
Environment Setup: Configured pandas, numpy, matplotlib, and seaborn with custom plotting themes.

Dataset Generation: Built synthetic data representing transaction records and computed Total_Sales.

Missing Data Handling: Injected 2% random missing values into Customer_Age and imputed them using median assignment (fillna).

Statistical Summarization: Derived mean, median, mode, standard deviation, min, and max for numeric features.

Visualization: Plotted distribution and relational graphs for revenue and customer demographics.

🛠️ Setup & Execution
Prerequisites
Ensure you have Python 3.8+ installed along with the required libraries:

Bash
pip install pandas numpy matplotlib seaborn
Running the Notebook
Launch Jupyter Notebook or JupyterLab:

Bash
jupyter notebook
Open the .ipynb file and run all cells sequentially.
