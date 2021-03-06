## Examples of relatively simple maps:

Cal Matters mapped [housing initiatives on the June ballot](https://calmatters.org/articles/map-how-we-voted-on-housing-issues-up-and-down-the-state/) -- Let's talk about how to make it more skimmable? Does this work and convey information, as a map?


## A Map to Remake

This was an interesting [quick hit on the rise of suicide](https://www.buzzfeed.com/carolinekee/suicide-rates-increase-us-2016-all-states) nationwide, but they used a map provided by the CDC, but really missed an opportunity to frame it.

**Title:** What is the takeaway? In the story, they captioned this "Suicide rates increased in almost all states between 1999 and 2016 — some by more than 30%.", but the chart uses "Figure. Percent change in annual suicide rate,* by state-- United States , from 1999/2001 to 2014/2016"

**Caption:** Tell me more about what I'm looking at. "A recent CDC report found that there is just one state in the union -- Nevada -- where suicides did not rise between 1999 and 2016."

**Map:** What are those buckets? If you look at this map where would you say the problem is most dramatic? This is a quantile map: they chose the buckets so that there are roughly the same number of states in each bucket. But one of these ranges is not like the others: 38-58% is a far bigger range. If we use "equal intervals," we wind up with very different buckets:

-1- 10.72
10.72 - 22.44
22.44 - 34.16
34.16 - 45.88
45.88 - 57.60

I think it makes some kind of sense to break it at zero, and at the national average (25.4)


The CDC report is based on raw data available in the CDC's [Morbidity and Mortality Weekly Report](https://www.cdc.gov/mmwr/index.html)



More thoughts: how many of you did not recognize this as a map of the United States? Some things we can leave off. "This map shows"

## A Map to Make

### Unsolved Homicides

https://www.washingtonpost.com/graphics/2018/investigations/unsolved-homicide-database/?utm_term=.a91216e2d03a

So let's filter out the data that we don't need and zoom in on our region.

https://github.com/washingtonpost/data-homicides

More sources for data on this: http://www.murderdata.org/p/blog-page.html

https://crime-data-explorer-master.fr.cloud.gov/

https://openjustice.doj.ca.gov/
https://ucr.fbi.gov/crime-in-the-u.s/2010/crime-in-the-u.s.-2010/clearances
KQED did a great job on this in 2012:
https://fusiontables.google.com/DataSource?docid=1xzpD8TzW5dnNQr-Lp_KZdAWHnB8Dh2Ms4eZlXgU#rows:id=1
story in 2013
https://ww2.kqed.org/news/2013/02/12/oaklands-other-homicide-crisis-unsolved-cases/



### Vulnerable Buildings
https://www.nytimes.com/2018/06/14/us/california-earthquakes-high-rises.html

https://www.usgs.gov/news/usgs-rolls-out-groundbreaking-earthquake-study-haywired-earthquake-scenario

https://pubs.usgs.gov/fs/2018/3016/fs20183016.pdf

Table 37 on page 360 of https://pubs.usgs.gov/sir/2017/5013/sir20175013iq.pdf (page 380 has some great bad charts)

Structural Engineers Association of Northern California (SEAONC) compiled the list

## Map Driven Stories that Are great
This piece on water contamination in Nova Scotia came out of a spatial join of well locations with areas with higher potential for arsenic contamination. It was a simple analysis that led to a compelling story.

https://signalhfx.ca/deadly-water/

### Review

Sex offenders:
In 2006, California voters passed [Prop 83](http://www.lao.ca.gov/ballot/2006/83_11_2006.htm), which requires registered sex offenders to live at least 2000 feet from any school or playground. In 2015, the state supreme court said the [blanket restriction was too broad](https://www.nbclosangeles.com/news/local/California-Loosens-Sex-Offender-Residency-Restrictions-297740931.html) and the law could only be applied to offenders whose crimes involved children.

Sex offender restrictions buffered around schools to show how much of a city is off limits. How would you map those?

Transit:
SB 827 died pretty quickly, but it would have established buffer zones around transit hubs and forced denser zoning as of right.
 So how would you map the impact of that bill? <https://transitrichhousing.org/> tried.



## Tutorials for Further Research
http://akanik.github.io/mapping-2017/

### Other Tools
* Tableau (Peter Aldhous has a good [intro walk through](http://paldhous.github.io/ucb/2016/intro-data/week4.html) in his course notes.)

http://www.padjo.org/tutorials/#mapping



    https://github.com/amandabee/CUNY-SOJ-data-storytelling/wiki/Tip-Sheet:-Geocoding
    https://github.com/amandabee/CUNY-SOJ-data-storytelling/wiki/Where-to-Find-Shapefiles
    http://amandabee.github.io/CUNY-data-skills/hands-on/mapping.html
