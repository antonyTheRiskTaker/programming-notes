# Summary of each episode

[Link for the tutorial series](https://www.youtube.com/playlist?list=PLZ1QII7yudbecO6a-zAI6cuGP1LLnmW8e)

1. Intro 
    - Why the creator made the course (automating backtesting is a reliable
      way to successful trading).

2. Preview
    - Preview of the course.

3. Part 1 - Account setup
    - Go throuh how to set up an Oanda demo account.
    - Where to access Oanda API key.
    - Where to get (demo) account number.

4. Part 2 - A REST API
    - Introduction to REST API and how it works.
    - JSON data format
    - How to use Postman to test APIs (I am using VSCode's Thunder Client
      extension).
    - Example API for learning calling APIs:
      https://jsonplaceholder.typicode.com/
    - Introduce GET, POST and DELETE HTTP methods.

5. Part 3 - Oanda API
    - Demonstrate how to get price data by calling the Oanda API
      (example: first 10 hourly prices of the EURUSD pair).
    - Also go through the account endpoints (example: check what tradable
      instruments are available for the demo account).

6. #4 - Environment setup
    - Teach you how to set up a Python virtual environment.
    - It is a good practice to set up a separate venv for each project.
    - Go through how to activate and deactivate a Python venv.
    - How to install Python packages using pip
    - Install requests, pandas, jupyter packages.
    - What VSCode extensions to use for Python development
    - Show how to use jupyter notebook on VSCode.
    - Demonstrate how to print strings on Python.
    - jupyter notebook is a good interactive, convenient way to start analysing
      and exploring data.
    - Later, we will begin to write fully-fledged Python scripts.
    - Test if you can manage to import Python libraries on the notebook.

7. #5 - Getting Candle data with Python!
    - Make `defs.py` to store crucial info.
    - Import requests and `defs.py` in the jupyter notebook (`test.ipynb`).
    - Create a session object to have a persistent connection to the Oanda
      API.
    - Set out the parameters to get candle price data for a specific instrument.
      through API calls.
    - Assemble the url for making API calls.
    - Use dict() to create a dictionary to hold parameters for API calls.
    - Use the get() method of the session object created earlier to make GET
      requests for price data.
    - The result of the GET request is stored in a variable called `response`.
    - Once the request is successful, you can access the response's status code,
      content in json format etc.
    - The code written so far will be reorganised into classes and objects in
      Python scripts.

8. #6 - Tradable instruments
    - Create a notebook called `instrument.ipynb`.
    - Store tradable instruments for the demo account in a file.
    - Assign the response of an API call of tradable instruments to a variable
      called `data`.
    - The response is formatted in json (in Python, it's a list holding
      more than a hundred of dictionary objects).
    - Create a new list that stores instrument data that is needed.
    - This is done through a for-loop (N.B. the tutorial uses `item` when
      writting for-loop code to generate a new instrument list. Bad naming,
      use `instrument` instead, as in `for instrument in instruments`.)
    - Apparently, the tutorial creator thinks the following info is necessary
      for backtesting forex trading strategies (in Oanda API):
          i. name
          ii. type
          iii. displayName
          iv. pipLocation (how many decimal places is price quoted with)
          v. marginRate
    - Now the pandas library is introduced.
    - We are going to turn the new instruments list into a dataframe (a
      table-like object from pandas).
    - The instruments dataframe is evaluated into a beautifully formatted
      table.
    - Store the dataframe in a pickle file.
    - A pickle is a binary zip format that is provided by pandas. It takes less
      space to save data in pickle files.
    - pandas provides a method to read pickle files and reformat them back to
      pandas dataframes.

9. #7 - Historical Candle Data
    - Save candles to a table, like what was done in `#6 - Tradable instruments`
      .
    - For each candle in the table, there is:
        i. date
        ii. volume
        iii. bid ohlc prices
        iv. mid ohlc prices
        v. ask ohlc prices
    - These data would be needed for backtesting.
    - In addition, a couple of price-related lists are made:
        i. `['mid', 'bid', 'ask']`
        ii. `['o', 'h', 'l', 'c']`
    - Using these two lists, 12 combinations are created, e.g. 'mid_o', 'mid_h',
      'mid_l', 'mid_c', etc.
    - The combinations are used to create column names for the candles table.
    - Only completed candles are collected.
    - Extract the 12 prices and store them as key-value pairs in a candle
      dictionary, along with volume and time values.
    - Create a dataframe using the prices list.
    - Save the dataframe in a pickle file for later use.

10. #8 - Collecting data for multiple pairs
    - Created a notebook called `save_candles.ipynb`.
    - Now we are going to save candles for currency pairs of the eight major
      currencies.
    - First, get all possible tradable combinations of these currency pairs.
    - The tuple evaluated by `ins_df.shape` is a tuple with two values. The
      first one refers to entries (or rows of the table), the second: columns.
    - (Created a `demo.ipynb` to learn how to read `df.shape`)
    - `ins_df.name.unique()` returns an array of tradable instruments.
    - A double for-loop is used to generate 64 currency pairs (including
      those that don't make sense).
    - Then filter out those untradable pairs.
    - The tutorial creator starts to introduce the concept of function, which
      allows developers to write repeatable codes.
    - The instructions that generate currency pairs are stored in a function,
      which can be used and called elsewhere.
    - For the purpose of this video, the functions we are going to make are
      simply meant to encapsulate codes that are used to create candle data
      in `#7 - Historical Candle Data`.
    - A function (`fetch_candles()`) that fetches candles from the Oanda API
      is written.
    - A function (`get_candles_df()`) that handles the response returned by
      `fetch_candles()` and creates a dataframe for the candle data is written.
    - A function (`save_file()`) that saves a dataframe (returned by
      `get_candles_df()`) to a file is written.
    - Finally, we want to create a function (`create_data()`) that brings all of
      these three functions together.
    - We will move all of these functions to Python scripts and classes.

11. #9 - Some Clean Up, what is "__main__"
    - A utility script `utils.py` is created to store helper functions.
    - In `utils.py`, functions that return filenames are written.
    - The concepts of `__name__` and `__main__` are explored.

12. #10 - Classes, a (very) quick primer
    - The concept of class (OOP) is introduced.
    - There are some functionalities in class that are useful for the purpose
      of backtesting trading strategies.
    - `__init__(self)` is the constructor of a class and it is called every
      time we make an instance.
    - The parameter `self` refers to an individual instance of the class.
    - There are also class-level methods and attributes that aren't attached to
      any instances.
    - Member variables are class attributes attached to a class instance; it can
      be initialised by the constructor.
    - `vars()` is a built-in function that when given a class instance as an
      argument will return member variables and their values in a dictionary.
    - `__repr__()` is another built-in method that comes with every class. It is
      called when we try to print a class instance from the outside. It is
      usually used to return info about the class instance, instead of its
      memory location.
    - To write a class method, precede the function declaration with
      `@classmethod`.
    - The `cls` parameter refers to the class itself, not an individual instance
      .
    - Class-level methods help organise different functionalities of an
      application.
    - An instrument class would have a class-level function that maybe loads all
      of the instruments. It can return a list of tradable instruments, as
      opposed to individual instruments.
    - However, a class instance can call a class-level method, so be careful.

13. #11 - Tradable instrument class
    - We are creating an Instrument class in this part of the tutorial.
    - `pipLocation` is handy in calculating things like pip differences.
    - Get the dataframe of tradable instruments using the `get_instruments_df()`
      class method.
    - `df.to_dict(orient='records')` returns a list of objects. Please go check
      out the pandas doc for clarity.
    - Classmethod `get_instruments_list` is created.
    - List comprehension is used to generate a list of `Instrument` instances
      from the result of `df.to_dict(orient='records')`.
    - In the end, we have created an Instrument class that generates instances
      with the five attributes about a tradable instrument
      (see `#6 - Tradable Instruments`).

14. #12 - Oanda API Class
    - A class is created to fetch and process data from the Oanda API.
    - In this context of this tutorial (building classes for forex backtesting),
      `if __name__ == '__main__'` is used to test class instances.
    - For the `fetch_candles()` method, the code is mostly from the
      `save_candles.ipynb` as demonstrated in
      `#8 - Collecting data for multiple pairs`.
    - The `fetch_instruments()` method is used to make HTTP calls for
      instruments, returning the data in json format ready for further
      processing.
    - The `fetch_instruments_df()` method converts the result of 
      `fetch_instruments()` into a pandas dataframe of tradable instruments.
    - Finally, the `save_instruments()` method saves the dataframe in a pickle
      file.

15. #13 - Converting Dataframe data types
    - Create a new jupyter notebook called `candle_plot.ipynb` where price data
      is plotted.
    - Import necessary modules.
    - Read the pickle file of a currency pair with a specific timeframe.
    - Run `df.info()` and you will see that the price data fetched from the
      Oanda API is actually of the string data type. It needs to be converted
      back to numerical before we can do any analysis with the candle data.
    - Identify the columns that we want to convert into numbers.
    - Use list comprehension to create a list of dataframe columns that filters
      out columns that don't need to be modified.
    - Use `.apply(pd.to_numeric)` to converted data of the desired columns into
      numeric type.

16. #14 - Plotting candles with Plotly!
    - Install plotly in your virtual environment and import it to use the
      package to create graphs.
    - Create a dataframe subset so that we won't plot a few thousands of
      candles.
    - Use the `.copy()` method to create a copy of the subset, instead of just
      a reference.
    - Use the `go.Figure()` and `go.Candlestick()` classes to plot your candles.

17. #15 - Styling Plotly candlestick charts
    - 