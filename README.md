# Weather-Data-Recorder-for-AgriWeather-Insights
AgriWeather Insights, a service provider for farmers, needs a tool to log weather data for crop planning.  This project aims to create a system for recording and analyzing daily weather conditions.
Weather Data Recorder for AgriWeather Insights
Overview
This project is a Python application developed for AgriWeather Insights, a service provider for farmers, to log and analyze daily weather data for crop planning. The application allows users to record weather data (date, temperature, and condition), ensures unique date entries, performs trend analysis using Pandas, and exports results to a CSV file. The application is designed to run in Google Colab, with functionality to download or generate a sample dataset.
Features

Data Entry: Add weather data (date, temperature, condition) with date validation to ensure correct format (YYYY-MM-DD).
Duplicate Prevention: Uses a set to store unique dates, preventing duplicate entries.
Data Analysis: Summarizes trends (e.g., average temperature, min/max temperatures, condition frequency) using Pandas.
Data Export: Exports raw and summarized data to CSV files, downloadable in Google Colab.
Dataset Acquisition: Automatically downloads a sample weather dataset from a public source (e.g., NOAA) or generates a sample dataset if needed.
Error Handling: Validates inputs to handle incorrect date formats or non-numeric temperatures.

Requirements

Python 3.x
Libraries:
pandas
requests (for downloading datasets)
datetime
google.colab (for Google Colab file handling)


Google Colab environment for running the notebook
Internet access for downloading external datasets (if applicable)

Installation

Clone the Repository:
git clone https://github.com/your-username/weather-data-recorder.git
cd weather-data-recorder


Set Up Google Colab:

Upload the weather_data_recorder.ipynb notebook to Google Colab.
Alternatively, open the notebook directly in Colab if shared via a link.


Install Dependencies:

The notebook includes code to install required libraries (pandas, requests) using !pip install in Colab.
Run the setup cell in the notebook to install dependencies automatically.



Usage

Open the Notebook:

Launch the weather_data_recorder.ipynb in Google Colab.


Run the Notebook:

Execute the cells in sequence to:
Download or generate the sample weather dataset.
Initialize the data storage and validation functions.
Add new weather data interactively using input prompts or Colab forms.
View recorded data and summarized trends.
Export data to CSV and download using Colab’s file handling.




Sample Workflow:

Run the dataset acquisition cell to download or generate data.
Use the provided functions to add new entries (e.g., 2025-09-01, 25.5, Sunny).
View data summaries (e.g., average temperature, condition counts).
Download the exported CSV files (weather_data.csv and summary.csv).


Example Output:

Raw data CSV: Contains columns for Date, Temperature, and Condition.
Summary CSV: Includes average temperature, min/max temperatures, and condition frequency.



Dataset

Source: The notebook includes code to download a sample dataset from a public source (e.g., NOAA’s daily weather data) or generate a sample dataset with 10+ days of data (e.g., dates, temperatures between 10–35°C, conditions like Sunny, Cloudy, Rainy).
Format: Data includes Date (YYYY-MM-DD), Temperature (float, in Celsius), and Condition (string, e.g., Sunny, Rainy).

Project Structure
weather-data-recorder/
│
├── weather_data_recorder.ipynb  # Main Google Colab notebook
├── README.md                   # Project documentation
└── sample_data/                # Optional folder for sample datasets (if downloaded)

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit (git commit -m "Add feature").
Push to the branch (git push origin feature-branch).
Open a pull request with a description of your changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.
Contact
For questions or support, contact Through Email [rajeshvulasala20@gmail.com] or open an issue on GitHub.
