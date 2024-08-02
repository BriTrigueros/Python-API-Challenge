# Python-API-Challenge

Certainly! Below is a template for your `README.md` file in GitHub format, detailing the steps and instructions for the Python API Challenge project.

---

# Python API Challenge

## Background

Data's true power is its ability to definitively answer questions. In this project, we will leverage Python requests, APIs, and JSON traversals to answer the fundamental question: "What is the weather like as we approach the equator?"

We will create visualizations to showcase the relationship between various weather variables and latitude. Additionally, we will plan future vacations using weather data skills, employing the Geoapify API and geoViews Python library for map visualizations.

## Before You Begin

### Repository Setup

1. Create a new repository called `python-api-challenge`.
2. Clone the new repository to your computer.
3. Inside your local Git repository, create a directory for this assignment called `WeatherPy`.
4. Add the provided starter files (`api_keys.py`, `WeatherPy.ipynb`, and `VacationPy.ipynb`) to this directory.
5. Create a `.gitignore` file to ensure sensitive information (like API keys) is not shared publicly.

### Adding a .gitignore File

1. Open your `python-api-challenge` GitHub folder in VS Code.
2. Open the `.gitignore` file and add the following:
   ```
   # Adding api_keys.py file.
   api_keys.py
   ```
3. Check the status of your repository:
   ```
   git status
   ```
4. Stage, commit, and push your changes:
   ```
   git add .gitignore WeatherPy.ipynb VacationPy.ipynb
   git commit -m "Initial commit with WeatherPy and VacationPy notebooks"
   git push origin main
   ```

## Files

Download the [Module 6 Challenge files](https://courses.bootcampspot.com/courses/629/files/782206/download) to get started.

## Instructions

This activity is broken down into two deliverables: `WeatherPy` and `VacationPy`.

### Part 1: WeatherPy

In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the `citipy` Python library, the OpenWeatherMap API, and your problem-solving skills to create a representative model of weather across cities.

1. **Generate random geographic coordinates and the nearest city to each latitude and longitude combination.**

2. **Retrieve Weather Data:**
   - Use the OpenWeatherMap API to retrieve weather data for the cities list generated.
   - Create a series of scatter plots to showcase the following relationships:
     - Latitude vs. Temperature
     - Latitude vs. Humidity
     - Latitude vs. Cloudiness
     - Latitude vs. Wind Speed

3. **Compute Linear Regression:**
   - Compute linear regression for each relationship.
   - Separate the plots into Northern Hemisphere (latitude >= 0) and Southern Hemisphere (latitude < 0).
   - Create scatter plots with linear regression lines, model's formula, and r^2 values.

### Part 2: VacationPy

In this deliverable, you'll use your weather data skills to plan future vacations. Use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

1. **Create a Map with City Data:**
   - Display a point for every city in the `city_data_df` DataFrame.
   - The size of the point should represent the humidity in each city.

2. **Narrow Down Ideal Weather Conditions:**
   - Filter the DataFrame to find your ideal weather conditions (e.g., max temperature between 21°C and 27°C, wind speed less than 4.5 m/s, zero cloudiness).

3. **Create a DataFrame for Hotels:**
   - Create a new DataFrame called `hotel_df` to store the city, country, coordinates, and humidity.
   - Use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
   - Add the hotel name and country as additional information in the hover message for each city on the map.

### Hints and Considerations

- The city data you generate is based on random coordinates and different query times, so your outputs will not be an exact match to the provided starter notebook.
- Study the OpenWeatherMap API to understand the request and response structure.
- The citipy library helps find the nearest city for given geographic coordinates.
- Ensure your repository has regular commits and a thorough `README.md` file.

### Summary

By completing this project, you'll gain a strong understanding of the core foundations of data analytics. Good luck!
