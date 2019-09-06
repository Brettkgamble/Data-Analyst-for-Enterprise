## Dataset
We have flight databases for 1992 (5020651 entries), 1998 (5227051 entries) and 2004 (6987729 entries) for the USA. The following characteristics are taken in account:

- `Total delay` which is a sum of `Arrival delay` and `Departure delay` in minutes
- `Distance` in miles
- `Month` (between 1...12)
- `CRS elapsed time` in minutes
- `Actual elapsed time` in minutes

## Summary of Findings

The total delay averaged per month is the highest on summer vacations period and in December. It's similar in all observed years.

The hypothesis of article [1] wasn't proved on our dataset. It assumes that CRS elapsed time is overestimated to be pessimistic, so that the delays are virtually less, which wasn't truth: first, they are not correlated, second, CRS elapsed time is quite accurate w.r.t. actual elapsed time.

Also the total delay turns out to be independent from distance, which is not surprising, because distance, CRS elapsed time and actual elapsed time are strongly correlated.

## Key Insigts of Presentation

First we highlight the distribution of total delay, which turns out to be unimodal, when one averages it per flight number.

Then we check if the total delay depends on distance, which turns out to be false.

We find the dependency of delays on month of the year, which is one of the findinds.

Also we verify the assumption in [1], which turns out to be false on our dataset.

## Files

- Flights.html - HTML report of **exploration**
- Flights.ipynb - original **exploration** notebook
- FlightsPresentation.ipynb - original **explanation** notebook
- FlightsPresentation.slides.html - **explanation** presentation in HTML format

The rest are supplementary scripts and a template file.
