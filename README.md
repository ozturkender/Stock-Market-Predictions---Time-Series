# Stock-Market-Predictions---Time-Series
Machine Learning at time series data with Linear Regression using Python Scikitlearn
In this project, we'll be working with data from the S&P500 Index. We'll be using historical time tagged data to make predictions about future prices. Data includes daily opening, highest of the day, lowest of the day and closeing indexes as well as volume of the days trade. Time frame is Jan 1, 1950 to Dec 7, 2015.

The columns of the dataset are:

- Date -- The date of the record.
- Open -- The opening price of the day (when trading starts).
- High -- The highest trade price during the day.
- Low -- The lowest trade price during the day.
- Close -- The closing price for the day (when trading is finished).
- Volume -- The number of shares traded.
- Adj Close -- The daily closing price, adjusted retroactively to include any corporate actions. Read more here.

Normal machine learning datasets are formed of independent incidents at each row. In this case, since the data is time-sequential, we should be extra careful not to inject future knowledge into past rows when doing the predictions. 

At time series problems, we should create indicators to make future predictions. When defining the values of these indicators, we should use the past data, but only the past not the data of the day since we cannot know any value of the day upfront when we predict future data.
