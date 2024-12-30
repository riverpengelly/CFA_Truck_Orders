# Chick-fil-A Inventory and Sales Automation Project

This project automates the processing of Chick-fil-A truck order data, enabling efficient tracking of inventory and sales trends. By leveraging Python, it converts truck order PDFs into organized Excel spreadsheets, aggregates monthly data, and provides insights to optimize operations.

## Features
- **PDF to Excel Automation**: Converts truck order PDFs into Excel files for easy data handling.
- **Data Aggregation**: Combines monthly data into a single spreadsheet, summarizing totals for inventory and sales trends.
- **Trend Analysis**: Identifies anomalies and trends in inventory costs, aiding in strategic decision-making.
- **Cost Optimization**: Tracks key items to minimize waste and improve operational efficiency.

## Technologies Used
- **Python Libraries**:
  - `pandas`: Data manipulation and aggregation
  - `tabula`: Extracting tabular data from PDFs
  - `os`: File and directory management
  - `logging`: Process tracking and debugging
  - `fuzzywuzzy`: String matching for description accuracy
  - `re`: Regular expressions for pattern matching
- **Excel**: Output format for processed data

## Workflow
1. **PDF Extraction**: Automatically reads truck order PDFs and extracts key information (e.g., item descriptions, supplier codes, quantities, and costs).
2. **Data Cleaning**: Cleans and organizes extracted data for consistency and accuracy.
3. **Aggregation**: Combines monthly data to identify trends and generate actionable insights.
4. **Optimization**: Analyzes data to reduce waste, track costs, and improve inventory management.

## Benefits
- Reduces manual workload for truck order processing (~5 minutes per batch).
- Improves data accuracy and accessibility.
- Provides actionable insights for cost reduction and operational efficiency.

## Usage
1. Place your PDF truck orders in the designated input folder.
2. Run the script to automatically generate Excel spreadsheets.
3. Review the aggregated monthly data for trends and insights.

## Future Enhancements
- Incorporating real-time data visualization.
- Adding machine learning models to predict inventory needs.
- Expanding functionality to handle additional data sources.

## Acknowledgments
This project was developed as part of my role as Back of House Team Leader at Chick-fil-A Sublett, in collaboration with the Executive Director. It is designed to enhance operational efficiency and support decision-making in a high-paced environment.

---

Feel free to explore the repository and contribute! If you have any questions or suggestions, please open an issue or reach out.
