# **Regression and Classification using AutoGluon**

## **Overview**
This project demonstrates the use of AutoGluon, an automated machine learning framework, for performing regression and classification tasks. The project focuses on analyzing weather data to predict temperature and classify wind speed across 17 Canadian cities. The workflows are designed to be simple, extensible, and highly effective.

---

### YData Profiling Report
To gain a better understanding of the dataset, we used **YData Profiling** to generate an exploratory data analysis (EDA) report. You can view the full **EDA Report** here: [Exploratory Data Analysis Report - Laptop Dataset](https://sandeepmondkar14.github.io/pages/combined_weather_report.html).

## **Project Goals**
1. **Regression Analysis**:
   - Predict the temperature using weather-related attributes such as humidity, pressure, and wind speed.
   - Evaluate the model's performance using metrics like RMSE and R².

2. **Classification Tasks**:
   - Classify cities into wind speed categories: `Calm`, `Breezy`, and `Windy`.
   - Analyze feature importance and the accuracy of the classification models.

3. **Reusable Framework**:
   - Provide reusable workflows for regression and classification tasks, which can be adapted for different datasets.

---

## **Dataset**
### The project uses the following CSV files:
- **Real-time weather data:** Data collected for 17 Canadian cities.
- **Historical hourly data:** Detailed weather observations over a historical period.
- **24-hour forecast:** Weather forecasts for the next day.
- **14-day forecast:** Weather predictions for a two-week period.

### Key Features of the Data:
- `temperature_celsius`: Actual temperature (°C).
- `feels_like_celsius`: Perceived temperature (°C).
- `humidity`: Percentage of atmospheric moisture (%).
- `pressure`: Atmospheric pressure (mbar).
- `wind_speed`: Wind speed (km/hr).
- `weather`: Description of weather conditions (e.g., few clouds, overcast).
- `city`: The location where weather data is recorded.

---

## **Setup Instructions**
### Prerequisites
- Python 3.11
- Required libraries:
  - pandas
  - scikit-learn
  - AutoGluon

### Installation
Install the dependencies:
   ```bash
   pip install pandas scikit-learn autogluon
   ```

## **How to Use**
1. **Download CSV Files**:
   - Download all the required CSV files from the repository.
   - Replace the file paths in the `.ipynb` notebooks with the paths to where you have stored the CSV files locally.

2. **Run the Jupyter Notebooks**:
   - Open the regression and classification `.ipynb` files in Jupyter Notebook or Jupyter Lab.
   - Execute the cells sequentially to load data, preprocess it, train models, and evaluate results.

3. **Analyze Results**:
   - Review regression outputs, including RMSE and R² scores.
   - Examine classified results for wind speed categories (`Calm`, `Breezy`, and `Windy`).

---

## **Key Features**
### **Regression**
- Predicts temperature using weather data attributes.
- Automated model selection and hyperparameter tuning with AutoGluon.

### **Classification**
- Classifies cities into categories based on wind speed:
  - **Calm**: Wind speed < 3 km/hr.
  - **Breezy**: Wind speed between 3 km/hr and 15 km/hr.
  - **Windy**: Wind speed > 15 km/hr.
- Evaluates model performance and highlights feature importance.

---

## **Example Outputs**
### Regression:
- The best model accurately predicts temperatures with minimal error, achieving high R² values.

### Classification:
- Example classification of cities by wind category:
  - **Calm**: Toronto, Ottawa
  - **Breezy**: Vancouver, Calgary, Halifax, and others
  - **Windy**: No cities meet this category in the provided dataset.

---

## **Limitations**
- Users must replace the CSV file paths in the `.ipynb` notebooks to their local paths for successful execution.
- The dataset is weather-specific, requiring adaptations for other use cases.

---

## **Future Enhancements**
- Add visualizations to display regression trends and classification distributions.
- Extend classification to include additional weather conditions (e.g., precipitation, cloud cover).
- Integrate seasonal data for deeper insights.

---

## **License**
This project is licensed under the MIT License. You are free to use, modify, and distribute the code.

---

## **Acknowledgments**
Special thanks to:
- **AutoGluon** for simplifying machine learning workflows.
- Openweathermap APIs for providing comprehensive weather data.

```
## Author
### Sandeep Mondkar
