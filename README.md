## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. This notebook will utilize Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, I know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how that assertion be **proved**?

![Equator](Images/equatorsign.png)

## WeatherPy

The Jupyter Notebook in this repository is a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, the notebook utilizes a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), and a little common sense to create a representative model of weather across world cities.

The ultimate objective is to build a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The final notebook will:

* Randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save both a CSV of all data retrieved and png images for each scatter plot.

As final considerations:

* This Jupyter Notebook includes the Matplotlib and Pandas plotting libraries.
* The notebook includes written descriptions of three observable trends based on the data.
