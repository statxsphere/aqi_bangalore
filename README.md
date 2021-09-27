# The Impact of COVID-19 Lockdowns on the Air Quality of Bangalore.

**The Blog post for this project can be found [here](https://shoobydo.substack.com/p/the-covid-lockdowns-were-a-breath).**

### Part 1: Performing hypothesis testing to determine change in air quality before and after travel restrictions:
A one-way F-test (ANOVA) was run on AQI grouped into pre and post travel restrictions.

### Part 2: Implementing a Recurrent Neural Network to forecast future AQI:
Due to its ability to retain sequential information, a Long-Short Term Memory Neural Network was implemented for this project.

### Objectives

* To explore trends in climate and AQI data in Bangalore.
* To understand the statistical importance of the travel restrictions on air quality.
* Implement a deep learning model to forecast future AQI and contrast forecasts made using pre-restriction data to forecasts made using post-forecast data.

### Data

* AQI Data - [Kaggle](https://www.kaggle.com/rohanrao/air-quality-data-in-india)
* Weather Data = [World Weather Online](https://www.worldweatheronline.com/developer/api/historical-weather-api.aspx)
* GIS Data - [OpenBangalore Github](https://github.com/openbangalore)

### Environment

1. Jupyter Notebook
2. Numpy
3. Pandas
4. Seaborn
5. Scipy
6. Keras
7. Tensorflow
8. Geopandas

The model achieved an RMSE of ~26 AQI.

### Areas of Improvement

1. Dataset - The dataset was restricted from 2015 - 2020, more data - especially data that includes the second lockdown as well would go a long way in improving the model.
2. Modelling - Due to computation reasons, the max number of features that were trained on were 10, and the max number of epochs was 2000, this could be tweaked to find more optimized parameters. Alternatively, different models like SARIMAX or ARIMAX could be used to make predictions as well.
