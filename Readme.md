Air Pollution Forecasting Project
Objective
This project aims to predict the Air Quality Index (AQI) for a city using time-series forecasting techniques, leveraging machine learning models like LSTM and ARIMA.

Dataset
The dataset contains air quality sensor readings with the following columns:

Date: The date of the observation.
Time: The time of the observation.
CO(GT): Carbon Monoxide concentration (Ground Truth).
PT08.S1(CO): Tin Oxide sensor readings.
NMHC(GT): Non-methane hydrocarbons concentration.
C6H6(GT): Benzene concentration.
PT08.S2(NMHC): Non-methane hydrocarbons sensor readings.
NOx(GT): Nitrogen Oxides concentration.
PT08.S3(NOx): Nitrogen Oxides sensor readings.
NO2(GT): Nitrogen Dioxide concentration.
PT08.S4(NO2): Nitrogen Dioxide sensor readings.
PT08.S5(O3): Ozone sensor readings.
T: Temperature.
RH: Relative Humidity.
AH: Absolute Humidity.
Steps
1. Data Handling
Loaded the dataset from an Excel file.
Combined Date and Time columns into a single Datetime column.
Handled missing values using forward fill and interpolation.
Set Datetime as the index for time-series operations.
2. Exploratory Data Analysis (EDA)
Analyzed trends and seasonality in the air quality data.
Visualized sensor readings over time.
3. Feature Engineering
Extracted features such as Hour, Day, and Month.
Calculated moving averages and rolling statistics.
Created lag features for time-series forecasting.
4. Model Training
Trained a Long Short-Term Memory (LSTM) model to predict AQI.
Compared LSTM's performance with a traditional ARIMA model.
5. Visualization
Plotted actual vs. predicted AQI values.
Created visualizations to highlight trends and anomalies.
Requirements
Python Libraries
Data Handling and Visualization:
pandas
numpy
matplotlib
seaborn
Machine Learning:
tensorflow
statsmodels
scikit-learn
Install the required libraries using:

bash
Copy code
pip install pandas numpy matplotlib seaborn tensorflow statsmodels scikit-learn
Usage
Clone the repository:
bash
Copy code
git clone https://github.com/itxmuhammadwaqarali/Air_quality_ndex.git
cd air-pollution-forecasting
Place the dataset file (air_quality_data.xlsx) in the project directory.
Run the main Python script:
bash
Copy code
python air_pollution_forecasting.py
Author
Muhammad Waqar Ali
Python Developer and Data Scientist
Contact: itxmewaqar@gmail.com
