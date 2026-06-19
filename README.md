# Olist E-Commerce Data Analysis 

## 1. General Summary of the Project
This project is a comprehensive data analysis study conducted on the public dataset of Olist, one of the largest e-commerce platforms in Brazil. The primary goal was to transform raw CSV data into a structured relational database, extract meaningful business insights using complex SQL queries, and visualize the findings to support data-driven decision-making. 

## 2. Key Findings
As a result of the SQL analyses, the following key insights regarding the platform's operations were obtained:
* **Market Domination:** The vast majority of the platform's customers are located in the **SP (Sao Paulo)** state. Focusing logistics and marketing investments in this region is of critical importance.
* **Revenue Leaders:** The product categories generating the highest revenue for the platform were **Health & Beauty** and **Watches & Gifts**, respectively.

## 3. Development Process
The project was developed in a systematic, step-by-step pipeline:
1. **Environment Setup:** Configured a local Git repository and established the folder structure while using `.gitignore` to keep data files out of version control.
2. **ETL Process & Schema Design:** Utilized Python to dynamically load CSV files into a local SQLite database. Additionally, created a `schema_design.sql` file to explicitly define table relationships using Primary and Foreign Keys.
3. **Data Analysis (SQL):** Formulated complex SQL queries involving aggregations (`GROUP BY`), multiple table merges (`JOIN`), and strict filtering (`WHERE` order_status = 'delivered') to answer specific business questions accurately.
4. **Data Visualization:** Converted the SQL query results into Pandas DataFrames and created informative charts using Matplotlib and Seaborn.

## 4. Challenging Parts of the Project
The most challenging aspects of the project included:
* Correctly mapping and joining three different tables (`order_items`, `products`, and `category_translation`) to calculate revenue per product category.
* Managing Python environment dependencies and resolving module import errors (e.g., ensuring `matplotlib` and `seaborn` were properly installed and recognized by the active Jupyter kernel).
* Designing clear and legible visualizations, specifically adjusting axes and formatting numbers to prevent scientific notation on large revenue figures.

## 5. Key Learnings
By the end of this project, I gained practical experience and learned:
* How to seamlessly transition between Python and SQL environments within a Jupyter Notebook.
* The importance of version control and how to effectively manage large datasets using `.gitignore`.
* How to turn raw database outputs into compelling visual stories that highlight key business metrics.

## 6. Roles of Technologies Used
* **Python:** Acted as the core engine for automation and data manipulation. It was used to read CSV files (via Pandas), execute SQL queries, and generate visual plots.
* **SQL (SQLite):** Served as the relational database management system. It played the critical role of establishing table schemas, joining distributed datasets, filtering specific business conditions (e.g., delivered orders), and aggregating metrics efficiently.
* **GitHub:** Played the essential role of version control and portfolio hosting. It tracked code changes systematically and provided a professional platform to present the final documentation and source code to evaluators.

## 7. Necessary Dependencies & How to Run
**Dependencies:**
To run this project, you need Python installed on your system along with the following libraries:
* `pandas`
* `matplotlib`
* `seaborn`

You can install them using the terminal:
`pip install pandas matplotlib seaborn`

**Instructions to Run:**
1. Clone this repository to your local machine.
2. Download the `Brazilian E-Commerce Public Dataset by Olist` from Kaggle.
3. Extract the downloaded CSV files into a folder named `data/` in the root directory.
4. Open the project in VS Code or Jupyter.
5. Run `1_data_transform.ipynb` first to create the SQLite database.
6. Run `2_sql_analysis.ipynb` to execute the queries and view the visualizations.

## 👨‍💻 Author

**Samet TÜRK**

* **Personal Email:** trksamet06@gmail.com
* **School Email:** 230201056@ostimteknik.edu.tr