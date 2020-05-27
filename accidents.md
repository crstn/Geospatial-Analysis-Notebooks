# 🏋 Exercise

> Which month of the year has the highest number of accidents?

There are a couple of ways to do this. Here is a very clean and self-explanatory version. First, we'll calculate the monthly sum of accidents:

```python
monthly_accidents = accidents['crash_count'].resample('M').sum()
```

Then we'll reformat the index so that it contains  [only the number of the month](https://docs.python.org/3/library/datetime.html#date-objects):

```python
monthly_accidents.index = monthly_accidents.index.month
``` 

Then we can ask for the row which contains the maximum value of the series:

```python
monthly_accidents[monthly_accidents == monthly_accidents.max()] 
``` 

If we want just the month number, we can do:

```python
maxmonth = monthly_accidents[monthly_accidents == monthly_accidents.max()].index[0]
maxmonth
``` 

And if we want to get really fancy, we can use the [calendar module](https://docs.python.org/3/library/calendar.html) to get the month name instead of just the number:

```python
import calendar
calendar.month_name[maxmonth]
```

¯\\\_(ツ)\_/¯