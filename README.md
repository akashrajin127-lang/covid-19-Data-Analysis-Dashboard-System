COVID-19 Data Analysis (Synthetic Data)
A Python project that generates synthetic COVID-19 data and produces a series of visualizations to explore trends across countries.

Overview
This script simulates COVID-19 case data for 8 countries over a 2-year period using the Faker library, then analyzes and visualizes the data using matplotlib, seaborn, and plotly.

Note: All data in this project is randomly generated and does not represent real-world COVID-19 statistics.


Features

Generates 500 synthetic records with Date, Country, Confirmed, Deaths, Recovered, and Active case fields
Computes summary statistics (totals for confirmed, deaths, recovered)
Produces 5 visualizations:

COVID-19 trend line (confirmed cases over time)
Bar chart of top countries by confirmed cases
Pie chart showing country-wise case distribution
Scatter plot of confirmed vs. deaths by country
Correlation heatmap across case metrics
Interactive Plotly trend line

Requirements
Install the required libraries before running:
bashpip install pandas numpy faker matplotlib seaborn plotly

How to Run
In Google Colab (recommended)

Open Google Colab
Upload the .py file or paste the code into a notebook cell
Run all cells — !pip install faker is already included in the script

Locally
bashpython python_project_7.py

Project Structure
python_project_7.py        # Main script — data generation + all visualizations

Data Schema
ColumnTypeDescriptionDatedatetimeRandom date within the last 2 yearsCountrystringOne of 8 countriesConfirmedintRandomly generated (1,000–100,000)DeathsintRandomly generated (10–5,000)RecoveredintRandom, capped at Confirmed countActiveintComputed: Confirmed − Deaths − Recovered
Countries included: India, USA, UK, Brazil, Germany, France, Italy, China

Visualizations
ChartLibraryDescriptionTrend LinematplotlibConfirmed cases aggregated by dateBar ChartseabornTotal confirmed cases per countryPie ChartmatplotlibCountry share of total casesScatter PlotseabornConfirmed vs. Deaths colored by countryHeatmapseabornCorrelation between Confirmed, Deaths, Recovered, ActiveInteractive LineplotlyZoomable/hoverable trend chart

