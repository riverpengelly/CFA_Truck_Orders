
# Chick-fil-A Truck Order Automation and Data Aggregation

This project automates the processing, aggregation, and organization of Chick-fil-A truck order data. By converting truck order PDFs into structured Excel files and generating monthly summaries, it streamlines inventory management and cost analysis.

## Features

- **Automated PDF Processing**: Extracts key data (e.g., supplier codes, item descriptions, quantities, unit costs, and total costs) from PDF files and converts them into Excel spreadsheets for easy analysis.

- **Data Cleaning and Validation**: Ensures descriptions are properly cleaned, numeric values are standardized, and logs warnings for incomplete or invalid rows to maintain data integrity.

- **Monthly Data Aggregation**: Combines data across files within a monthly directory, summarizing total quantities and costs per item, along with total monthly cost calculations.

- **Centralized Data Organization**: Organizes all processed and summarized data into respective directories and consolidates monthly summaries into a central folder for streamlined reporting.

- **Scalable Workflow**: Handles multiple directories (e.g., monthly subfolders) in batch processing mode, accommodating large datasets efficiently.

## File Structure

The repository is organized as follows:

```
CFA_Truck_Order_Automation/
├── src/                       # Python scripts for processing and aggregation
│   ├── process_pdfs.py        # Extracts and processes PDF data
│   ├── aggregate_months.py    # Aggregates data across monthly directories
│   ├── organize_summaries.py  # Collects all monthly summaries into a central folder
│
├── data/                      # Input and output directories for processing
│   ├── input/                 # PDF files for each month
│   └── output/                # Processed Excel files and summaries
│
├── README.md                  # Documentation and setup guide
├── requirements.txt           # Python dependencies
└── .gitignore                 # Ignore unnecessary files
```

## Libraries Used

The following Python libraries are utilized in this project:

- **`os`**: Handles directory and file operations.

- **`re`**: Provides regular expression support for pattern extraction and text cleaning.

- **`pandas`**: Enables data manipulation and analysis, including creating and aggregating dataframes.

- **`pdfplumber`**: Parses PDF files to extract tabular data.

- **`logging`**: Logs information, warnings, and errors to track script execution.

- **`shutil`**: Manages file operations, such as copying and moving files.

- **`openpyxl`**: Reads and writes Excel files (`.xlsx`).

- **`fuzzywuzzy`**: Matches strings approximately to ensure accurate description matching.

- **`python-Levenshtein`**: Speeds up string matching calculations (optional dependency for `fuzzywuzzy`).

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/riverpengelly/CFA_Truck_Orders.git
   cd CFA_Truck_Orders
   ```

2. **Install Dependencies**:
   Install the required Python libraries listed in `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare Input Data**:
   Place your truck order PDF files in the designated `data/input/` directory.

4. **Run the Scripts**:
   - **Process PDFs**: Converts PDFs into Excel files.
     ```bash
     python src/process_pdfs.py
     ```
   - **Aggregate Monthly Data**: Combines data into monthly summaries.
     ```bash
     python src/aggregate_months.py
     ```
   - **Organize Summaries**: Collects all monthly summaries into a central folder.
     ```bash
     python src/organize_summaries.py
     ```

## Benefits

- **Time Efficiency**: Automates manual data entry tasks, saving valuable time.

- **Data Accuracy**: Improves data consistency and reduces errors.

- **Actionable Insights**: Provides comprehensive reports for informed inventory and cost management decisions.

## Future Enhancements

- **Data Visualization**: Integrate tools for interactive dashboards.

- **Predictive Analytics**: Add features for inventory demand forecasting.

- **Extended Format Support**: Expand compatibility to include additional data formats (e.g., CSV).

## Acknowledgments

This project was developed as part of my role as Back of House Team Leader at Chick-fil-A Sublett. It demonstrates how automation and data-driven approaches can enhance operational efficiency and decision-making.

---

Feel free to explore the repository, suggest improvements, or contribute!
