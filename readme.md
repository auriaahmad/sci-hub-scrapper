# Scraper Project

This project is designed to scrape research papers using DOIs provided in an Excel file. Follow the instructions below to set up and run the code.

## Prerequisites

- Anaconda (for managing the Python environment)
- A stable internet connection

## Setup Instructions

### 1. Create and Activate Conda Environment

First, create a new conda environment:

```bash
conda create --name scraper-env python=3.8
```
```bash
conda activate scraper
```
### 2. Install Requirements

Navigate to the project directory and install the required packages:


```bash
pip install -r requirements.txt
```

### 3. Change Directories and Set Paths

Set the directory paths in the script where the downloads and the Excel file will be stored:

```bash
download_directory = r"<path of dir where you want to download pdfs>"
```

```bash
excel_file = r"<write path of doi.xlsx file with name and extension>"
```
Ensure your DOI Excel file (doi_updated.xlsx) is located in the root directory of the project.

### 4. Select Proper Interpreter
Make sure to select the appropriate Python interpreter that corresponds to the scraper-env conda environment in your IDE.

### 5. Run the Script
Run the script and keep it running. Ensure your internet connection is stable throughout the process.

### Notes
- The script does not handle all scenarios of errors.
- It does not handle DDoS detection; you must handle this manually if it occurs.

### After Downloading Papers
Once the desired list of papers has been downloaded:

- Remove the contents of the downloads directory and the updated_doi.xlsx file.
- Replace the DOI list in the Excel file with a new list of  papers you wish to download.
- Repeat the process to download the new set of papers.

### License
This project is licensed under the MIT License. This software comes as it is with not warrenty and maintanece. 