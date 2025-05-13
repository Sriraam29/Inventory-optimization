# Inventory-optimization
Calculation Stock Notebook
Overview
The calculation_stock.ipynb Jupyter Notebook demonstrates how to calculate the recommended stock for a fictional beverage distribution center. Using Python and pandas, it performs inventory analysis to optimize stock levels, minimize overstocking, and prevent stockouts. The notebook leverages ABC and XYZ analysis, safety stock calculations, and Economic Order Quantity (EOQ) to provide actionable insights.
Key Features

Data Loading and Cleaning: Imports and cleans six CSV files containing purchase, sales, and inventory data.
ABC Analysis: Classifies items by value (A, B, C) to prioritize high-value products.
XYZ Analysis: Assesses demand predictability (X, Y, Z) to understand sales patterns.
Safety Stock and EOQ: Calculates buffer stock and optimal order quantities.
Recommended Stock: Determines ideal stock levels, identifying overstock (2.7M units) and understock (284K units) with a potential 49.7% stock reduction.

Dataset
The notebook uses data from the Kaggle dataset Inventory Analysis Case Study by Bhanu Pratap Biswas. It includes:

InvoicePurchases12312016.csv: Vendor purchase invoices.
EndInvFINAL12312016.csv: Ending inventory.
SalesFINAL12312016.csv: Sales data.
BegInvFINAL12312016.csv: Beginning inventory.
2017PurchasePricesDec.csv: Purchase prices.
PurchasesFINAL12312016.csv: Purchase details.

Prerequisites

Python 3.10+
Jupyter Notebook or JupyterLab
Required Python libraries:pandas
numpy
seaborn
matplotlib
kagglehub



Installation

Clone the Repository:
git clone https://github.com/your-username/your-repo.git
cd your-repo


Install Dependencies:
pip install pandas numpy seaborn matplotlib kagglehub


Authenticate Kaggle (for dataset download):

Install the Kaggle CLI: pip install kaggle
Set up your Kaggle API key as described in the Kaggle API documentation.
Alternatively, manually download the dataset from the Kaggle link and place the CSV files in the notebook's directory.



Usage

Open the Notebook:
jupyter notebook calculation_stock.ipynb


Run the Cells:

Execute the cells sequentially to load, clean, and analyze the data.
Ensure the CSV files are in the same directory as the notebook or update file paths if needed.
The notebook downloads the dataset via kagglehub if not already present.


Key Outputs:

Total stock: 4,885,776 units
Total understock: 284,803 units
Total overstock: 2,712,878 units
Recommended stock: 2,457,701 units (49.7% reduction)



Structure
The notebook is organized into seven steps:

Load, Clean, and Wrangle Data: Imports and prepares the dataset.
Initial Observations: Explores data characteristics.
ABC Analysis: Categorizes items by value.
XYZ Analysis: Evaluates demand stability.
Calculate Safety Stock: Determines buffer stock.
Calculate EOQ: Computes optimal order quantities.
Calculate Recommended Stock: Combines analyses for final stock recommendations.

Results
The analysis reveals significant overstocking (especially in A and X classes) and understocking (notably in C and Y classes). By adopting the recommended stock levels, the distribution center can reduce inventory by nearly 50%, improving efficiency and reducing costs.
Contributing
Contributions are welcome! Please:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Commit your changes (git commit -m "Add feature").
Push to the branch (git push origin feature-branch).
Open a pull request.



Dataset provided by Bhanu Pratap Biswas.
Built with Python, pandas, and Jupyter.

Contact
For questions or feedback, reach out via sriraamhari04@gmail.com or open an issue on GitHub.
