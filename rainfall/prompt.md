# AI-Based Rainfall Prediction Dashboard (Real-Time Weather Experience)

You are a Senior Full Stack AI Engineer, Senior Machine Learning Engineer, Data Scientist, Streamlit Expert, Python Developer, and UI/UX Designer.

Build a **single-page AI Rainfall Prediction Dashboard** that provides a real-time weather application experience. The machine learning model should work entirely in the background. **Do not display any technical machine learning information such as model names, RMSE, MAE, R² score, feature importance, training time, prediction time, or algorithm selection.**

The application should feel like a commercial weather forecasting platform.

---

## Objective

Predict **Annual Rainfall** using a pre-trained machine learning model.

Dataset Columns:

* SUBDIVISION
* YEAR
* JAN
* FEB
* MAR
* APR
* MAY
* JUN
* JUL
* AUG
* SEP
* OCT
* NOV
* DEC

Target:

Annual Rainfall

The model is already trained and stored as **best_model.pkl**.

The dashboard should only load the model and generate predictions.

---

# Design Inspiration

Design similar to:

* Google Weather
* Apple Weather
* AccuWeather
* Microsoft Weather

Use a **light theme**.

Colors:

* Sky Blue
* White
* Soft Grey
* Cloud Blue
* Green accents

The interface should be minimal, elegant, modern, and clean.

---

# Dashboard Layout

## Header

* Project Logo
* AI Rainfall Prediction
* Current Date
* Search Location
* Light Theme

---

## Prediction Form

Subdivision Dropdown

Year Input

Monthly Rainfall Inputs

January

February

March

April

May

June

July

August

September

October

November

December

Buttons

* Predict Rainfall
* Reset
* Load Sample Data

---

## Prediction Results

After clicking **Predict**, instantly display:

### Main Prediction Card

* Predicted Annual Rainfall (mm)

### Rainfall Category

Automatically classify as:

* Low Rainfall
* Moderate Rainfall
* Heavy Rainfall
* Very Heavy Rainfall

Display matching weather icons and colors.

---

## AI Weather Summary

Generate a natural-language summary.

Example:

"Based on the rainfall values entered, the predicted annual rainfall is **1654 mm**. This indicates a **Heavy Rainfall** region. Such rainfall generally supports strong monsoon conditions and is favorable for many seasonal crops."

Do not mention machine learning or algorithms.

---

## Interactive Charts

Update automatically after prediction.

Include:

* Monthly Rainfall Bar Chart
* Monthly Rainfall Line Chart
* Monthly Rainfall Area Chart
* Annual Rainfall Gauge
* Rainfall Distribution Chart

Use Plotly for smooth interactive charts.

---

## Prediction Insights

Display easy-to-understand insights such as:

* Wettest Month
* Driest Month
* Average Monthly Rainfall
* Total Rainfall Entered
* Seasonal Trend

Present these as attractive weather cards.

---

## Recent Predictions

Maintain a history of predictions using Streamlit Session State.

Display:

* Date
* Subdivision
* Year
* Predicted Annual Rainfall
* Rainfall Category

Allow users to:

* Download history as CSV
* Clear history

---

## User Experience

The dashboard should behave like a live weather application.

When Predict is clicked:

* Validate inputs
* Show a loading animation
* Display a smooth progress indicator
* Animate the result cards
* Update charts dynamically
* Show a success notification

Prediction should appear instantly.

---

## Streamlit Components

Use:

* st.container()
* st.columns()
* st.metric()
* st.form()
* st.selectbox()
* st.number_input()
* st.button()
* st.spinner()
* st.progress()
* st.success()
* st.warning()
* st.error()
* st.plotly_chart()
* st.dataframe()
* st.download_button()
* st.session_state
* @st.cache_resource

---

## Performance

* Load the trained model only once.
* Use caching for preprocessing.
* Perform predictions in real time.
* Use relative file paths.
* Fully compatible with Streamlit Community Cloud.

---

## Code Quality

Generate clean, modular, production-ready code with:

* Reusable components
* Input validation
* Exception handling
* Logging
* Documentation
* Responsive design
* Accessibility support
* Fast loading
* Smooth animations

The machine learning model must remain completely hidden from users. The dashboard should provide a seamless, real-time weather prediction experience where users simply enter rainfall values, click **Predict Rainfall**, and immediately receive an intuitive forecast, visualizations, and easy-to-understand insights without any technical ML details.
