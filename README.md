 Analysis and Visualization of Pharmaceutical Spending Data (2018–2022)

 Overview
This project involves analyzing and visualizing pharmaceutical spending data from 2018 to 2022 using **Power BI**. The analysis explores spending trends, dosage units, and claims across various drug brands and manufacturers. An interactive dashboard was developed to highlight insights, such as the top spending brands, growth patterns, and outliers, aiding stakeholders in informed decision-making.

 Features of the Power BI Dashboard
The Power BI dashboard contains several interactive and insightful visualizations:
1. Clustered Column Chart
   - Visualizes total spending (2018–2022) by drug brand.
   - Reveals leading contributors such as Humira(Cf) Pen and Biktarvy.

2. Manufacturer Details Table
   - Displays total manufacturers, manufacturer names, and their total spending.
   - Identifies key manufacturers like Aurobindo Pharm and Mylan.

3. Scatter Chart
   - Plots the compound annual growth rate (CAGR) of average spending per dosage unit.
   - Highlights drugs with the highest CAGR, such as Glipzide.

4. Line Chart
   - Tracks average spending per dosage unit by brand over the years.
   - Shows pricing trends for brands like Supprelin LA and Ilanis.

5. Stacked Bar Chart
   - Visualizes total spending (2018–2022) by manufacturers.
   - Reveals spending trends and dependence on specific manufacturers.

6. Pie Chart
   - Displays the proportion of dosage units by brand.
   - Highlights high-usage brands like Sodium Chloride.

7. Slicers for Brand and Manufacturer
   - Enable data filtering based on specific brands or manufacturers.
   - Provide granular insights for targeted analysis.

8. Stacked Column Chart
   - Visualizes total claims (2018–2022) by generic drug names.
   - Identifies high-demand generics like Ibuprofen and Albuterol Sulfate.

Objectives
The project aims to:
1. Analyze spending trends and patterns in pharmaceutical data.
2. Highlight key insights such as outliers, growth trends, and spending by manufacturers.
3. Provide actionable insights to policymakers and stakeholders for financial planning and market strategy.

Dataset
The dataset contains 36 columns and 13,380 rows, with key attributes such as:
- `Brand_Name`
- `Generic_Name`
- `Total_Spending_2018–2022`
- `Total_Dosage_Units_2018–2022`
- `Total_Claims_2018–2022`
- `Avg_Spending_Per_Dosage_Unit_Weighted_2018–2022`
- `Outlier_Flag_2018–2022`

 Methodology

### Data Preparation and Transformation
1. **Fixing Data Types**: Ensured columns have correct data types (e.g., numeric, date).
2. **Renaming Columns**: Simplified column names for readability.
3. **Handling Missing Data**: Removed rows with null values in critical fields.
4. **Adding Custom Columns**: Added a `Year-over-Year Change` column for analyzing trends.

### Data Model
1. **Fact Table**:
   - Contains transactional data like spending, dosage units, and claims.
2. **Dimension Tables**:
   - Drug Dimension: Details of drug brands and generics.
   - Manufacturer Dimension: Manufacturer details and total spending.
   - Outlier Dimension: Flags for identifying outliers across years.
3. **Relationships**:
   - Established many-to-one relationships between the fact table and dimension tables.

## Key Insights
1. **Top Spending Brands**: 
   - Humira(Cf) and Biktarvy dominate total spending.
2. **Growth Patterns**:
   - High CAGR drugs, such as Glipzide, indicate rising costs.
3. **Outliers**:
   - Significant year-over-year spending changes from 2021 to 2022 signal areas for cost-saving or adjustments.

---

## Installation and Usage

### Prerequisites
- Microsoft Power BI Desktop
- Python (optional for preprocessing, if needed)

### Steps to Use
1. **Clone the Repository**:
   git clone https://github.com/yourusername/pharma-spending-analysis.git
   cd pharma-spending-analysis
2.	Open Power BI File:
3.	Explore Dashboard:
o	Use interactive slicers and visualizations to analyze spending trends and patterns.
________________________________________
Project Structure
plaintext
CopyEdit
├── README.md                  # Project documentation
├── data/                      # Dataset folder
│   └── pharmaceutical_spending.csv
├── src/                       # Data preparation and transformation scripts
│   ├── data_cleaning.py
│   ├── data_transformation.py
├── dashboard/                 # Power BI dashboard
│   └── ds331labproject_dashboardformatfinal044.pbix
├── reports/                   # Formal project report
│   └── DS331_project_report.pdf


Contributors
•	Adina Kamran (2022044)
GIK Institute of Engineering Sciences and Technology
Faculty of Data Science

References
•	Power BI Documentation: Microsoft Power BI
•	Pharmaceutical Data Analysis Techniques: Research articles and datasets.

