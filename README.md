# sales-report-a8b3d

## Brief
This project updates the sales report by adding a dynamic table that displays each product along with its total sales amount. The table is inserted into the webpage with the ID `#sales-table`. The data is sourced from a CSV file named `sales.csv`. Additionally, the total sales figure shown in the element with ID `#total-sales` remains accurate after the update.

---

## Features
- Parses `sales.csv` to extract sales data.
- Generates a table with headers `Product` and `Sales`.
- Calculates total sales per product, rounded to 2 decimal places.
- Updates the sales report dynamically without page reload.
- Ensures the total sales element (`#total-sales`) reflects the correct total after the update.

---

## Setup Instructions
1. **Clone the repository** or download the project files to your local machine.
2. Ensure that the `sales.csv` file is placed in the project directory or update the script to point to the correct location.
3. Open the `index.html` file in your preferred web browser to view the sales report.

*No additional dependencies are required; the script uses vanilla JavaScript.*

---

## Usage Guide
- The script automatically runs on page load.
- It reads the `sales.csv` file, processes the data, and dynamically populates the table with ID `#sales-table`.
- The total sales figure displayed in the element with ID `#total-sales` will be updated to reflect the sum of all sales.

**Note:** Ensure that the CSV file is correctly formatted, with each line containing a product name and sale amount separated by a comma, e.g.:

```
Product1,123.45
Product2,67.89
```

---

## Technical Details
- **Language:** JavaScript (ES6+)
- **Libraries:** None (vanilla JavaScript)
- **CSV Parsing:** Simple line split; no external CSV parsing library used.
- **Data Handling:** Calculates per-product total sales and overall total.
- **HTML Structure:** Assumes an existing element with ID `#sales-table` for insertion.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize further or reach out if you need additional features!