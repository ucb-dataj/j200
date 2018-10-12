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


------------------------

# Cal Fire
Cal Fire publishes fire hazard zones --
http://www.fire.ca.gov/fire_prevention/fire_prevention_wildland_zones_maps

Lisa Pickoff-White did some nice work for the KQED coverage of the northbay fires. [Bay Area Fire Hazard](https://ww2.kqed.org/science/2017/10/31/map-see-if-you-live-in-a-high-risk-fire-zone-and-what-that-means/)

We can actually download the map.  http://www.fire.ca.gov/fire_prevention/fire_prevention_wildland_statewide

## In Mapbox
Add it as a tileset -- because it is a full shapefile.

## In Datawrapper
They only accept a few file types for upload so we're going to [follow their advice](https://academy.datawrapper.de/article/145-how-to-upload-your-own-map) and let [Mapshaper](https://mapshaper.org/) do some of the heavy lifting.
* Upload the zipfile
* use the `i` button to confirm that shapes have data attached (note: it looks like maybe the fire zones lack unique IDs?) -- we can fix this with dissolve? 
* Project into the WGS-84 coordinate system. More on map projections: https://xkcd.com/977/
