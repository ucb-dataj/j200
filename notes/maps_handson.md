Walkthrough.


CDC Suicide:
The raw data is available at:
https://www.cdc.gov/vitalsigns/suicide/infographic.html#graphic1


Select "USA States" in Datawrapper, click "next"

Look at the data: do we have ISO codes or names?

Import -- find the csv. it should automatically recognize the abbreviations

---------------------

Unsolved Homicides

* I reordered the columns with
`csvcut -c 10,11,1-9,12 homicide-data_oakland.csv > dw_homicides_oakland.csv` to make them easier to work with.

`csvcut -c reported_date,uid morsel.csv | in2csv -f fixed -s morsel.schema > morsel_dates.csv` to break the dates in to year, month, day

`csvjoin -c uid morsel.csv morsel_dates.csv` to join them by uid.
