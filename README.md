# Sensor Data Processing

## Project Overview

This project processes sensor readings from multiple devices and generates:

1. A daily summary containing:
   - Number of valid readings per day
   - Average reading per day
    
2. Device-specific files containing all readings for each device.

## Input Data Format

device_id,date,reading

Example:

00731,2024-03-01,42
0147,2024-03-02,N/A
3563,2024-03-02,

## Output Files

- daily_summary.csv
- 00731.csv
- 0147.csv
- 3563.csv

## Approach

- Read the sensor data using Pandas
- Convert readings to numeric values
- Exclude invalid values (N/A and blanks) from calculations
- Generate daily summary statistics
- Create separate files for each device

## Technologies Used

- Python
- Pandas
- Google Colab

## How to Run

1. Open the notebook in Google Colab.
2. Run all cells.
3. Generated files will be saved automatically.
