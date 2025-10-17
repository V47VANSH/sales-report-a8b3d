# sales-report-a8b3d

## Brief Description
This project updates the sales report webpage by adding a detailed table that displays each product and its corresponding sales amount from a CSV data source. The table with the ID `#sales-table` includes a header row (`Product`, `Sales`) and dynamically populated data. Additionally, the total sales element with the ID `#total-sales` remains accurate after the update.

---

## Features
- Parses sales data from `sales.csv`.
- Displays a table with product names and their total sales.
- Maintains an accurate total sales figure.
- Rounds sales amounts to 2 decimal places.
- Responsive and easy to integrate into existing reports.

---

## Setup Instructions
1. Ensure your project directory contains the `sales.csv` file with sales data formatted as:
    ```
    Product,SaleAmount
    Product A,123.45
    Product B,67.89
    ...
    ```
2. Include the JavaScript code responsible for processing the CSV and updating the table and total sales element. This script should run after the DOM has fully loaded.
3. Make sure your HTML contains the following elements:
    ```html
    <table id="sales-table"></table>
    <div id="total-sales"></div>
    ```
4. Link your JavaScript file in your HTML:
    ```html
    <script src="path/to/your/script.js"></script>
    ```

---

## Usage Guide
1. Load your webpage in a browser.
2. The script will automatically:
    - Read `sales.csv`.
    - Populate the `#sales-table` with product names and sales amounts.
    - Calculate and display the total sales in `#total-sales`.
3. The table will have headers "Product" and "Sales" and rounded sales figures to two decimal places.
4. Verify that the total sales display reflects the sum of all individual sales.

---

## Technical Details
- The script uses the Fetch API to load `sales.csv`.
- Parses CSV data into an array of objects.
- Aggregates sales per product if multiple entries exist for the same product.
- Creates and inserts a table dynamically into the DOM.
- Handles rounding to two decimal places for sales figures.
- Ensures the total sales value updates correctly after data processing.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

*Thank you for using the sales report update! For any issues or feature requests, please open an issue in this repository.*