Zuber — Chicago Taxi Ride Analysis
Objective

Zuber, a new ride-sharing company launching in Chicago, needs to understand passenger preferences and the impact of external factors on rides. This project analyzes taxi trip data (retrieved via SQL and exported as CSV) to identify the most active taxi companies and the neighborhoods with the highest number of drop-offs, and tests whether average ride duration from the Loop to O'Hare International Airport changes on rainy Saturdays.

Result

The number of rides is unevenly distributed across taxi companies, with a few companies concentrating most of the market share, and certain neighborhoods receiving significantly more drop-offs than others. A t-test (α = 0.05) on ride duration between rainy and clear Saturdays returned a p-value below 0.05, rejecting the null hypothesis: ride duration from the Loop to O'Hare is statistically significantly different on rainy Saturdays.

Tools

Python, Pandas (data loading, filtering, sorting, grouping), Matplotlib (bar charts), SciPy (ttest_ind for hypothesis testing), SQL (used upstream to generate the CSV extracts).

What I learned

This project connected SQL-extracted data with a full Python statistical workflow, reinforcing how to formulate and test a hypothesis about the effect of an external factor — weather — on a business metric like ride duration.

Possible improvements

Extend the hypothesis test to other routes and days of the week to check whether the weather effect on ride duration is specific to the Loop–O'Hare route or a broader citywide pattern.

Data

This project uses three CSV extracts produced by SQL queries against the trip and weather database
