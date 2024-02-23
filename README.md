# Algerian Forest Fire Prediction


## lab-flask

<!-- ![image](https://user-images.githubusercontent.com/115451707/196919992-edcfea8b-e3f6-4f35-9398-43be66b5622d.png) -->


To run flask application 

```
python app.py
```


To access your flask application open new tab in and paste the url:
```
https://{your_url}.app:5000/
```


## Overview
Forest fires are a major concern worldwide, and Algeria is one of the countries affected by these phenomena, particularly during the summer. Detecting and forecasting forest fires are critical for minimizing damage. This project aims to predict whether or not a fire will break out based on weather data.

## Features Used for Prediction
- **Temperature (Temp):** Noon temperature (maximum temperature) in Celsius degrees (ranging from 22°C to 42°C).
- **Relative Humidity (RH):** Percentage of relative humidity (ranging from 21% to 90%).
- **Wind Speed (Ws):** Wind speed in km/h (ranging from 6 km/h to 29 km/h).
- **Rain:** Total rainfall during the day in mm (ranging from 0 mm to 16.8 mm).
- **FWI Components:**
  - **FFMC (Fine Fuel Moisture Code):** Index from the Fire Weather Index (FWI) system (ranging from 28.6 to 92.5).
  - **DMC (Duff Moisture Code):** Index from the FWI system (ranging from 1.1 to 65.9).
  - **DC (Drought Code):** Index from the FWI system (ranging from 7 to 220.4).
  - **ISI (Initial Spread Index):** Index from the FWI system (ranging from 0 to 18.5).
  - **BUI (Buildup Index):** Index from the FWI system (ranging from 1.1 to 68).
  - **FWI (Fire Weather Index):** Overall fire danger index (ranging from 0 to 31.1).

## Additional Information
- **Classes:** The predicted classes (e.g., fire occurrence or no fire occurrence).
- **Region:** The specific region or area in Algeria where the prediction is applicable.

## Trained Models
- `scaler.pkl`: Trained Random Forest model.
- `ridge.pkl`: Trained Ridge Regression model.

## Deployment Platform
The project is deployed on Amazon Web Services (AWS) for real-time predictions.

## Project Structure
- **app.py:** Main Python script for running the prediction model.
- **requirements.txt:** List of required Python packages.
- **templates:** Folder containing HTML templates for the web application.


## Usage
1. Install the required packages using `pip install -r requirements.txt`.
2. Run `app.py` to start the web application.
3. Input weather data (temperature, humidity, wind speed, rainfall) to get the fire prediction result.

## Acknowledgments
This project was developed as part of the effort to improve forest fire prevention and management in Algeria.

