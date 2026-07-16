# Hotel Booking Analysis

This project contains an exploratory data analysis (EDA) script for hotel booking data. The analysis is performed in `hotel_booking_analysis.py` and uses Python libraries such as `pandas`, `matplotlib`, and `seaborn` to inspect booking patterns, cancellations, and pricing trends.

## Project Files

- `hotel_booking_analysis.py` - Main analysis script generated from a Colab notebook.

## Dataset

The script uses a CSV file named `hotel_bookings 2.csv` located in the same directory as the script.

> Note: The dataset file is provided with this project, so you can run the analysis immediately after installing the dependencies.

## Analysis Overview

The notebook performs the following steps:

- Loads the hotel booking dataset into a `pandas` DataFrame
- Inspects the data structure and summary statistics
- Converts `reservation_status_date` to datetime format
- Removes columns `company` and `agent` if present
- Drops missing values
- Removes outliers in `adr` values above 5000
- Generates visualizations to explore:
  - Booking cancellation percentages
  - Cancellation rates by hotel type
  - Average Daily Rate (ADR) trends over time for Resort Hotel and City Hotel
  - Monthly booking cancellations
  - ADR for canceled bookings by month
  - Top 10 countries with booking cancellations

## Requirements

Install the required Python packages before running the script:

```bash
pip install pandas matplotlib seaborn
```

## Running the Analysis

Run the script from the project directory:

```bash
python hotel_booking_analysis.py
```

If you want to use the notebook form of this analysis, the script was originally generated from a Colab notebook.

## Notes

- The script uses `warnings.filterwarnings('ignore')` to suppress warnings.
- The analysis is exploratory and does not save output files; it displays plots in a Python environment.
- Ensure the dataset file is available and named exactly `hotel_bookings 2.csv`.
