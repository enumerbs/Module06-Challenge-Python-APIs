# Module06-Challenge-Python-APIs
Data Analytics Boot Camp - Module 06 - Python APIs \
Python APIs Challenge

---

# Results

Refer to the following Jupyter Notebook files:
### Part 1: WeatherPy
*WeatherPy/WeatherPy.ipynb*

### Part 2: VacationPy
*VacationPy/VacationPy.ipynb*

# Implementation notes

Part 1: WeatherPy
- Open Weather API
    - Obtain current weather data based on details at https://openweathermap.org/current
- Scatter Plots
    - Added import for 'datetime' module, to be able to interpret 'Unix epoch' datetime UTC value returned by the API - and so add the date the weather measurements were retrieved to the Title of each scatter plot.
    - In 'starter code' .ipynb file, the Title on the first scatter plot was "City Max Latitude vs. Temperature (2024-06-17)" but I think the position of 'Max' was a typo, and it should have been "City Latitude vs. Max Temperature (2024-06-17)", to align the terminology with the y-axis label. I've adjusted the Title for the first scatter plot accordingly in my case.
- Linear Regression
    - Linear regression calculation code adapted from earlier module: Module 05 'Data Visualisation', Lession 5.3 'Introduction to Statistics'
    - Linear regression equation text overlay adapted from Module 05, Lession 5.3, Activity '08-Ins_Fits_and_Regression'.

Part 2: VacationPy
- Hvplot - scatter plot catgories, and specifically colours per category can apparently be specified be either the 'by' parameter (for grouping) or the 'color' parameter. The 'by' approach gave an error to do with NdOverlay, so the 'color' parameter was the better option in this case. Refer to the refence below for more details.

# References

The following references were used in the development of the solution for this Challenge.

## Matplotlib - text annotation on plots
- https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.annotate.html

## Unix epoch datetime values
- https://note.nkmk.me/en/python-unix-time-datetime/

## Hvplot - scatter plot points' colour control
- https://stackoverflow.com/questions/56484779/holoviews-scatter-plot-color-by-categorical-data