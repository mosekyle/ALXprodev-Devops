# ALXprodev-Devops

# Advanced Shell Scripting: Automating Tasks and Managing Processes

This repository contains scripts that automate various tasks using shell scripting. The tasks involve making API requests, processing data, and handling errors efficiently. Below are the details of the tasks in this project.

## Tasks Overview

### 1. API Request Automation
- **Objective**: Automate the process of making an API request to the Pokémon API and saving the response to a JSON file (`data.json`). If the request fails, the error is logged to `errors.txt`.
- **Script**: `apiAutomation-0x00`

### 2. Extract Pokémon Data
- **Objective**: Extract specific data (name, height, weight, and type) from the `data.json` file using advanced text manipulation tools (`jq`, `awk`, `sed`), and format the output in a human-readable way.
- **Script**: `data_extraction_automation-0x01`

### 3. Batch Pokémon Data Retrieval
- **Objective**: Automate the retrieval of data for multiple Pokémon and store it in separate files named after the Pokémon (e.g., `pikachu.json`, `bulbasaur.json`). Handle rate-limiting issues by adding a delay between requests.
- **Script**: `batchProcessing-0x02`

### 4. Summarize Pokémon Data
- **Objective**: Create a report summarizing the data for multiple Pokémon, including their name, height, and weight. The script will also generate a CSV file and calculate the average height and weight using `awk`.
- **Script**: `summaryData-0x03`

### 5. Error Handling and Retry Logic
- **Objective**: Enhance the script from Task 2 by adding error handling and retry logic. The script will retry a failed request up to 3 times before logging the error and moving on to the next Pokémon.
- **Script**: `batchProcessing-0x02`

### 6. Parallel Data Fetching
- **Objective**: Speed up data retrieval using parallel processing. This script will fetch data for multiple Pokémon concurrently by leveraging background processes and process management tools.
- **Script**: `batchProcessing-0x04`

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/Advanced_shell.git
   cd Advanced_shell
   ```

2. **Make the scripts executable**:
   ```bash
   chmod +x apiAutomation-0x00 data_extraction_automation-0x01 batchProcessing-0x02 summaryData-0x03 batchProcessing-0x04
   ```

3. **Run the scripts**:
   - For Task 1 (API Request Automation):
     ```bash
     ./apiAutomation-0x00
     ```
   - For Task 2 (Extract Pokémon Data):
     ```bash
     ./data_extraction_automation-0x01
     ```
   - For Task 3 (Batch Pokémon Data Retrieval):
     ```bash
     ./batchProcessing-0x02
     ```
   - For Task 4 (Summarize Pokémon Data):
     ```bash
     ./summaryData-0x03
     ```
   - For Task 5 (Error Handling and Retry Logic):
     ```bash
     ./batchProcessing-0x02
     ```
   - For Task 6 (Parallel Data Fetching):
     ```bash
     ./batchProcessing-0x04
     ```

## Requirements
- `curl` - For making API requests.
- `jq` - For processing JSON data.
- `awk`, `sed` - For text manipulation.
- `bash` - For scripting.
