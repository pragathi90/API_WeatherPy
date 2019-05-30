# API_WeatherPy
Homework 6 - Weather Py 

#WeatherPy
#Your objective is to build a series of scatter plots to showcase the following relationships:
#Temperature (F) vs. Latitude
#Humidity (%) vs. Latitude
#Cloudiness (%) vs. Latitude
#Wind Speed (mph) vs. Latitude

#You must include a written description of three observable trends based on the data.
### Observable Trends

1. Temperature (F) vs. Latitude

*In the Temperature vs. Latitude scatter plot, as the latitude increases the temperature increases, which means that the temperatures which are higher the closer they are to the equator. 

However, temperature peaks at around 30 degrees latitude and the max temperature is around 105 degrees. Temperature drops to around 20 degrees which gives us the min temperature and that's around 65 latitude. 

Latitude has direct affect on the temperatures which means temperatures does show a strong correlation to latitude. 

-----------------------------------------------------------------------------------

2. Humidity (%) vs. Latitude

Latitude has no direct affect on the humidity directly which means Humidity does not show a strong correlation to latitude.
Humidity is more directly related to temperatures,which we can have more concluded results if we were to plot this against temperatures rather than against Latitude.


-----------------------------------------------------------------------------------


3. Cloudiness (%) vs. Latitude
Latitude has no direct affect on the cloudiness directly which means Cloudiness does not show a strong correlation to latitude.
Cloudiness is more directly related to temperatures,,which we can have more concluded results if we were to plot this against temperatures rather than against Latitude.

-----------------------------------------------------------------------------------

4. Wind Speed (mph) vs. Latitude
Latitude has no direct affect on the windspeed directly which means Wind Speed does not show a strong correlation to latitude.
Wind Speed is more directly related to temperatures,,which we can have more concluded results if we were to plot this against temperatures rather than against Latitude.

Wind speed appears to slightly increase as we move away from the equator.
In the Wind Speed (mph) vs. Latitude scatter plot, the average when speed for all cities is fairly low. 
The wind speeds are higher on average at the north and south poles.


.........................................................................




In this example, I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 
To accomplish this, I used a simple Python library [simple Python library](https://pypi.python.org/pypi/citipy) , the OpenWeatherMap API [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.


The objective is to build a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude



* Humidity (%) vs. Latitude



* Cloudiness (%) vs. Latitude



* Wind Speed (mph) vs. Latitude



Languages and Tools: 
- Python
- Pandas
- Numpy
- Requests
- Citipy
- API Calls
- Matplotlib
- Seaborn

# Dependencies and Setup
import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
import time
import json
import requests as req
import random
import seaborn as sns
import math as math
import openweathermapy as owm

# Import API key
from api_keys import api_key

# Incorporated citipy to determine city based on latitude and longitude
from citipy import citipy

#import datetime to label the graphs
from datetime import datetime