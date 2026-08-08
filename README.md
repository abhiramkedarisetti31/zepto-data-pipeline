# Module 1 - Data Pipeline

## Install & Run Steps
1. Upload the `.ipynb` file to Google Colab.
2. Run the cells sequentially to scrape the data, build the database, and execute the SQL queries.
3. The pipeline generates a local SQLite file named `zepto_pipeline.db` (which is also included in this repository).

## Design Decisions
* **Currency Conversion**: The baseline conversion rate used is exactly **1 GBP = 105.50 INR** as mandated by the assignment.
* **Data Cleaning**: Rows missing crucial numeric data (like price or rating) are dropped from the dataset rather than imputed. Because this is a pricing intelligence pipeline, inserting fake median prices would ruin the integrity of the data benchmark.
