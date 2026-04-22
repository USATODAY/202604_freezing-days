# Freezing days analysis

## Results

We analyzed temperature data for the past seven decades to see how winters in major cities have changed. 

We found almost all cities analyzed (255/257) are now experiencing fewer freezing days per season compared to the mid 1950s -- with 86% of cities losing at least a week of freezing days. In addition, these warming cities:

- On average are now experiencing 19 fewer freezing days per water year.
- Freezing days on average are starting 11 days later and ending 26 days earlier for a shorter cold season. 
- The longest streak of freezing days in a water year is also 12 days shorter on average.
- The coldest day of the water year has also warmed an average of 5.6 degrees Fahrenheit.

In short, the freezing season is becoming shorter and milder.

This is based on an analysis of climate data spanning 1956-2025. We extracted daily minimum temperature from the center of every city with a population over 100,000. We then ran linear regressions on those that had at least one freezing day in at least half the years.

For more details on our methods, you can run the `methods.Rmd` file or go through the notebook here: https://usatoday.github.io/202511_freezing-days/methods.html

## Outputs

- `total_change_city.csv` and `total_change_county.csv`: summarizes the change between 1956 and 2025 by location across different metrics like the number of freezing days per water year and a few others
- `yearly_stats_city.csv` and `yearly_stats_county.csv`: timeseries that describes the metrics by water-year summarized in `total_change_city` and `total_change_city`

## Inputs

The raw climate data is extracted through the script itself. The first time running it takes lots of time to download all the files, but intermediate files are also saved to reduce processing time on subsequent local runs.

## Citation

If you use this data, please cite it and [link to the published project](https://www.usatoday.com/graphics/interactives/how-climate-change-is-impacting-winters/). Citation suggestion below:
 
“1956-2025 Freezing Days Analysis.” *USA Today*, https://www.usatoday.com/graphics/interactives/how-climate-change-is-impacting-winters/. Accessed [date accessed]."

## Credits

Code written by Ignacio Calderon, USA Today Data Reporter. For any questions, reach out at [icalderon@usatoday.com](icalderon@usatoday.com)