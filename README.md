# Chick-fil-A Truck Order Automation and Data Aggregation

This project automates the processing, aggregation, and organization of Chick-fil-A truck order data. It streamlines inventory management and cost analysis by converting truck order PDFs into structured Excel files, generating monthly summaries, and consolidating data for efficient trend analysis.

## Features

1. **Automated PDF Processing**:
   - Extracts key data (e.g., supplier codes, item descriptions, quantities, unit costs, and total costs) from PDF files.
   - Converts data into Excel spreadsheets for easy manipulation and analysis.

2. **Data Cleaning and Validation**:
   - Ensures descriptions are properly cleaned and numeric values are standardized.
   - Logs warnings for incomplete or invalid rows, maintaining data integrity.

3. **Monthly Data Aggregation**:
   - Combines data across files within a monthly directory.
   - Summarizes total quantities and costs per item, with a total monthly cost calculation.

4. **Centralized Data Organization**:
   - Organizes all processed and summarized data into respective directories.
   - Consolidates monthly summaries into a central folder for streamlined reporting.

5. **Scalable Workflow**:
   - Handles multiple directories (e.g., monthly subfolders) in batch processing mode.

## File Structure

The repository is organized as follows:

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


## Technologies Used
## Libraries Used

The following Python libraries are used in this project:

1. **`os`**  
   - Handles directory and file operations (e.g., creating and navigating folders).

2. **`re`**  
   - Provides regular expression support for extracting patterns (e.g., supplier codes) and cleaning text.

3. **`pandas`**  
   - Enables data manipulation and analysis, including creating and aggregating dataframes.

4. **`pdfplumber`**  
   - Parses PDF files to extract tabular data.

5. **`logging`**  
   - Logs information, warnings, and errors to track script execution.

6. **`shutil`**  
   - Manages file operations, such as copying and moving files.

7. **`openpyxl`**  
   - Reads and writes Excel files (`.xlsx`).

8. **`fuzzywuzzy`**  
   - Matches strings approximately to ensure accurate description matching.

9. **`python-Levenshtein`**  
   - Speeds up string matching calculations (optional dependency for `fuzzywuzzy`).

### Installation

These libraries can be installed using the `requirements.txt` file. To install all dependencies, run:

```bash
pip install -r requirements.txt
```
**Excel**: Output format for processed data

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
