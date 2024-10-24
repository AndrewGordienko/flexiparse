<img src="https://github.com/user-attachments/assets/f246be23-ed44-4e88-a0a8-e4dd8f9afab2" alt="image" width="300"/>

# OpenSearch Data Export Tool

The Flexiparse library is a Python script designed to parse dynamically and export data from the OpenSearch JSON API responses into a structured CSV format. It automates the process of extracting and transforming unstructured JSON data from OpenSearch into a well-formatted DataFrame, which can then be exported for further analysis or reporting.

## Features

- **Dynamic Field Extraction:** Recursively parses JSON responses from OpenSearch without hardcoding specific fields, making it reusable for different types of data and reports.
- **Customizable Column Ordering:** Dynamically orders DataFrame columns based on field priority, with special handling for volume and metric columns.
- **CSV Export:** Exports parsed data into CSV files for further manipulation, tracking, or alerting systems.

## Installation

Install the library and dependencies via `pip`:

```bash
pip install flexiparse
```

Ensure the following dependencies are installed:

- `pandas`

## Usage

The documentation is in documentation.ipynb.

## Input Files

### Request File

- The request file should contain the OpenSearch aggregation query. This is used to map field names and understand the structure of the response.

### Response File

- The response file contains the OpenSearch aggregation results. The script dynamically processes these results into a table format.

### Output

- The output will be a CSV file structured similarly to the visualization in your OpenSearch GUI, making it easy to import the data into other systems for analysis.

## Project Structure

- **main.py:** The core script containing logic to process and export OpenSearch data.
- **request.json:** Example request file containing the OpenSearch query structure.
- **response.json:** Example response file containing the aggregation results.
- **output.csv:** The CSV output generated by the script.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
