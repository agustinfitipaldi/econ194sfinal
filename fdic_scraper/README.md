# FDIC State Tables Scraper

This script automates the process of downloading FDIC state tables data for all 50 states from 2019 onwards.

## Prerequisites

- Python 3.7 or higher
- Firefox browser installed
- pip (Python package installer)

## Installation

1. Create a virtual environment (recommended):
```bash
python3 -m venv venv
source venv/bin/activate  # On Linux/Mac
# or
.\venv\Scripts\activate  # On Windows
```

2. Install the required packages:
```bash
pip3 install -r requirements.txt
```

## Usage

Simply run the script:
```bash
python3 fdic_scraper.py
```

The script will:
1. Open a headless Firefox browser
2. Iterate through all 50 states
3. Download data for each state from 2019 onwards
4. Combine all data into a single CSV file named `fdic_all_states_data.csv`

## Notes

- The script includes a 1-second delay between states to be respectful to the server
- If the script encounters any errors with a particular state, it will log the error and continue with the next state
- The final CSV will include a 'State' column to identify the data source
- The script runs in headless mode (no visible browser window)

## Troubleshooting

If you encounter any issues:
1. Make sure Firefox is installed and up to date
2. Check that you have a stable internet connection
3. Verify that your Downloads folder is accessible
4. If you get timeout errors, you may need to increase the wait times in the script 