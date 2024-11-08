# Module 6 Challenge

## Overview 
This challenge is split into two parts, the "WeatherPy" challenge and the "VacationPy" challenge. A detailed overview of each is provided below. 

## WeatherPY

In this challenge, we use the "citipy Python library" and "OpenWeatherMap API" to create a representative model of weather across cities. To do so, we create a Python script to visualize the weather of over 500 cities at varying distances from the equator.
    
## Objectives
    
    Step 1: Use the OpenWeatherMap API to gather weather data from the cities list generated in the starter code and create plots to show the relationship between the latitude of a city and the following weather variable: 
        1. Latitude vs. Max Temperature 
        2. Latitude vs. Humidity 
        3. Latitude vs. Cloudiness 
        4. Latitude vs. Wind Speed 
    Step 2: Seperate plots into Northern Hemisphere and Southern Hemisphere and calculate the linear regression for each of the following: 
        1. Northern Hemisphere: Temperature vs. Latitude
        2. Southern Hemisphere: Temperature vs. Latitude
        3. Northern Hemisphere: Humidity vs. Latitude
        4. Southern Hemisphere: Humidity vs. Latitude
        5. Northern Hemisphere: Cloudiness vs. Latitude
        6. Southern Hemisphere: Cloudiness vs. Latitude
        7. Northern Hemisphere: Wind Speed vs. Latitude
        8. Southern Hemisphere: Wind Speed vs. Latitude

## VactionPY

For the "VactionPy" challenge we use Jupyter notebooks, the "geoViews Python library", and the Geoapify API to create map visualization that will help us plan our next vacation. In this assignment, we create a map that shows a point for every city in the "city_data_df". We then narrow down the list of cities by filtering the data frame to only include the cities with our ideal weather conditions. In this case, those conditions are a temperature between 27 degees (C) and 21 degrees (C), a wind speed less than 4.5 m/s, and 0% cloudiness. 

## Files
 - "python-api-challenge"(git@github.com:jackthomas1430/python-api-challenge.git): The main repo for this challenge. 
    - "output_data" folder: contains the the "cities.csv" exported through the "WeatherPy.ipynb" python script and images of the plots created during our analysis.  
        - “cities.csv”: the csv file containing the cities and weather data gathered through the "WeatherPy.ipynb" python script
    - "WeatherPy_VacationPy" folder: contains all files needed for the module 6 challenge 
        - "VactionPy.ipynb": the main script for the "VactionPy" challenge
        - "WeatherPy.ipynb": the main script for the "WeatherPy" challenge 
    
## Set Up
    
    1. Clone the repository to your local device using git clone https://github.com/jackthomas1430/python-api-challenge.git
    2. Sign up for API Keys using the following links: 
        weather_api_key: https://home.openweathermap.org/users/sign_up
        geoapify_key: https://myprojects.geoapify.com/register
    3. Add API keys to api_keys.py and save (add api_keys.py to the .gitignore file before pushing changes to Github)
    
    4. To run the script, you will need to complete the following installations: 
    

      " 1. Open Anaconda Prompt (in Windows) or a Terminal window (in macOS).

        2. Activate your virtual environment by typing `conda activate dev` and pressing Enter.

        3. To install the [GeoViews](https://geoviews.org/), run:

        ```shell
        conda install -c pyviz hvplot geoviews
        ```

        > **Note** For some installations, you might get a message indicating that the requested packages are already installed. This is fine&mdash;Conda automatically installs the software dependencies that these libraries require.
        To make sure these libraries installed properly, run:

        ```shell
        conda list hvplot
        conda list geoviews
        ```

        If you do not see anything listed when you check the `geoviews` library, you may try an alternative install option. Run the following:

        ```shell
        conda install -c conda-forge geoviews
        
        5. To install [citypy](https://github.com/wingchen/citipy), which is needed for the challenge, run:

        ```shell
        pip install citipy
        ```

        After installing these libraries, restart Jupyter notebook if it was running. Recall that you must launch Jupyter Notebook from your Python environment for these libraries to work.

>       **Note:** GeoViews relies on several packages that may cause conflicts with your base             Python environment, which is why it is important to install these libraries only within         your `dev` environment.```" (Installation instructions provided by course instructors)
    5. Run "WeatherPY.ipynb"
    6. Run "VacationPy.ipynb"
    
## Summary/Analysis 
    The "WeatherPy" analysis shows that latitude has a moderate impact on the maximum temperature of the cities in our dataset. The linear regression plots show that as we move further away from the equator the temperatures typically decrease. The data does not suggest that latitude has a strong influence on any of the other weather conditons: humidity, cloudiness, and wind speed. Ultimately, this analysis supports the notion that the closer to the equator you are the hotter it will be.  
    The "VactionPy" script narrowed my list of potential destinations down 10 cities based on my ideal whether conditions. Inerestingly, 5 of the 10 cities were in Mexico and there were 4 cities in which there was no hotel within 10,000 meteres found through the search. Considering I have never heard of and certainly cannot pronouce the majority of the cities on the list, the Comfort Rooms in Cabo San Lucas, Mexico is where you will find me on my next vacation. 
##Acknowledgements
    
    Xpert Learning Assistant was used to answer detailed questions, and assist in debugging.The starter code provided was the base of the report and was modified using course curriculum and activities to fit the requirements of the assignment. The TA and instructor for the course also assisted in adjusting the code during office hours.For more information about the Xpert Learning Assistant, visit [EdX Xpert Learning Assistant](https://www.edx.org/). 

## References

1. Python min() and max() Functions. (n.d.). Real Python. Retrieved from https://realpython.com/python-min-and-max/
2. citipy. (n.d.). PyPI. Retrieved from https://pypi.org/project/citipy/
3. Geoapify Forward Geocoding API. (n.d.). Geoapify. Retrieved from https://apidocs.geoapify.com/docs/geocoding/forward-geocoding/#about
4. Geoapify API Documentation. (n.d.). Geoapify. Retrieved from https://apidocs.geoapify.com/
5. Current Weather Data. (n.d.). OpenWeather. Retrieved from https://openweathermap.org/current
6. Python Try Except. (n.d.). W3Schools. Retrieved from https://www.w3schools.com/python/python_try_except.asp
7. scipy.stats.linregress. (n.d.). SciPy Documentation. Retrieved from https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html
8. pandas.plotting.scatter_matrix. (n.d.). pandas Documentation. Retrieved from https://pandas.pydata.org/docs/reference/api/pandas.plotting.scatter_matrix.html
9. pandas.DataFrame.plot. (n.d.). pandas Documentation. Retrieved from https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.html
10. Weather API. (n.d.). OpenWeather. Retrieved from https://openweathermap.org/api
    About Geographic Coordinate Systems. (n.d.). ArcGIS. Retrieved from https://desktop.arcgis.com/en/arcmap/10.3/guide-books/map-projections/about-geographic-coordinate-systems.htm
11. Introduction to hvPlot. (n.d.). hvPlot Documentation. Retrieved from https://hvplot.holoviz.org/user_guide/Introduction.html
12. matplotlib User Guide. (n.d.). Matplotlib Documentation. Retrieved from https://matplotlib.org/stable/users/index.html


Data for this dataset was generated by edX Boot Camps LLC

© 2022 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
Data generated by MockarooLinks to an external site., LLC (2022). Realistic Data Generator.
