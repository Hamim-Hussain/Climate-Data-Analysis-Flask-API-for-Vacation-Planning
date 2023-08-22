# Climate Data Analysis & Flask API for Vacation Planning
<img src="images/surf.jpg" width="1000" height="491">


## Introduction
Planning a relaxing vacation in Honolulu, Hawaii? Here's how to analyse the climate data and design a Flask API to help make your trip unforgettable.

## Part 1: Climate Data Analysis
Utilise Python, SQLAlchemy, Pandas, and Matplotlib to explore climate data and gain insights. Follow these steps using the provided files (climate_starter.ipynb and hawaii.sqlite):

1. Connect to the SQLite database with create_engine().
2. Reflect tables into classes using automap_base() and create references for station and measurement.
3. Establish a SQLAlchemy session to interact with the database.

### Precipitation Analysis:

1. Identify the most recent date in the dataset.
2. Retrieve the last 12 months of precipitation data from this date.
3. Select only "date" and "prcp" values.
4. Load query results into a Pandas DataFrame and set the index to "date".
5. Sort DataFrame values by "date".
6. Create a plot of the results using the DataFrame plot method.
7. Print summary statistics for the precipitation data.

### Station Analysis:

1. Calculate the total number of stations in the dataset.
2. Identify the most-active station (highest observation count).
3. List stations and observation counts in descending order.
4. Design a query to calculate the lowest, highest, and average temperatures for the most-active station.
5. Obtain the previous 12 months of temperature observation (TOBS) data for the most-active station and plot it as a histogram.

## Part 2: Designing a Climate App
After completing the data analysis, create a Flask API with the following routes:

1. /: Start at the homepage and list all available routes.
2. /api/v1.0/precipitation: Retrieve the last 12 months of precipitation data and return it as a JSON dictionary.
3. /api/v1.0/stations: Return a JSON list of stations from the dataset.
4. /api/v1.0/tobs: Query temperature observations for the most-active station from the previous year and return a JSON list.
5. /api/v1.0/<start> and /api/v1.0/<start>/<end>: Return a JSON list containing minimum, average, and maximum temperatures for specified date ranges. For a single start date or a start-end range.

With this climate data analysis and Flask API, you can confidently plan your vacation in Honolulu. Explore historical weather patterns and access valuable insights to make the most of your trip!'





