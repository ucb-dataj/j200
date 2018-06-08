Very rough notes for Amanda on reading, story starting points, etc.

* https://mjwebster.github.io/DataJ/Other/WrestlingWithData.pdf

* where does 

Good local data story: 
https://www.nytimes.com/2018/05/12/upshot/these-95-apartments-promised-affordable-rent-in-san-francisco-then-6580-people-applied.html



And replies to a call for "entry level" data stories: 
--------
## Payday Lending
Find some data. 

## Civil Forfeiture
https://boingboing.net/2018/06/01/i-am-the-law-2.html

## Nuisance abatement

Sarah Ryeley: My series on nuisance abatement that won a Pulitzer didn't really go much those tools. I did some of the analysis in Tableau, but you could probably do the same with pivot tables. It was probably the simplest data story I've ever done, in terms of the tools needed for the actual analysis. The harder part was the process behind the data collection, and then of course the rest of the reporting. I have a more detailed blow-by-blow of the process in my IRE entry, which is in the IRE library. But I use this series as an example at the end of my beginners data bootcamp and my "Intro to Data Tools" presentation to show that you can still get big impact by incorporating even basic data skills into your investigations :)
+ https://www.propublica.org/article/propublica-new-york-daily-news-pulitzer-public-service-nuisance-abatement#more-about-this-reporting

Dan Telvock: My two-part series on a badly polluted creek that was an IRE finalist a few years ago used pivot tables in Excel to calculate number of sewer overflow, which water received the poo and which localities were responsible. I also developed my own spreadsheet for the volumes for one of the localities by requesting all of their overflow reports sent to the state. In the end, it helped build context and the case that this creek is unhealthy. *Warning: second video is a bit disturbing for some, I am sure. *

http://www.investigativepost.org/2014/07/17/the-scajaquada-crippled-creek/
http://www.investigativepost.org/2014/07/24/disgust-outrage-scajaquada-creek/

Alex Brockman:  Here's a relatively simple data-driven story that we did at CBC Windsor a couple years ago. http://www.cbc.ca/news/canada/windsor/south-windsor-intersection-speeding-1.3762090 It did take an FOIA request from the local police force to get the data, but it only took a month to get. I got an excel dataset with the location and date of speeding tickets handed out over the past five years. After a few sorts, pivot tables, and some work with Google Fusion tables, we found the most-ticketed intersection and used it as a newshook into an in-depth profile of the person who lived at that corner. 

We also published an interactive tool with Google Maps that was a standalone element: http://www.cbc.ca/news/canada/windsor/speeding-tickets-windsor-1.3762141

## Jaywalking Tickets 

Two of my most fun data-driven stories happened when I was at the Columbus Dispatch in Ohio (miss you, Ohio public records laws). One looked at where people were getting ticketed (and when) for jaywalking <http://www.dispatch.com/content/stories/local/2014/06/15/dozens-of-jaywalking-tickets-issued-in-city-each-month.html>.
I did that after a big jaywalking enforcement blitz. The other looked at public urination citations <http://www.dispatch.com/article/20141201/NEWS/312019688> (and involved one of my favorite police quotes ever, "You don't buy beer, you rent it.") Both of these had maps I made in Google Fusion, but a website redesign wiped them out.

## Claims against the City 
http://www.yakimaherald.com/news/local/lawsuits-claims-just-the-cost-of-doing-business-for-yakima/article_e076d9ae-0978-11e8-a4b8-9bcb976cdac5.html

## Technique 
Patrick Cain: 

1) find the biggest/smallest outlier in a data set, and;
2) Go find out why that thing is the way it is.

Two Toronto examples: the Star had a story a while back from the city's
noise complaint database about the most-complained-about property in the
city (this turned out to be a compelling account about neighbour conflict
with a really callous nighclub owner) and a CP story from the city parking
ticket database about the hydrant that had the most tickets for parking in
front of a fire hydrant (it turned out to be in an odd place and really
hard to see.)

Teaching a class like that, I'd toss them a big database and challenge them
to find stories in it, while also offering suggestions and guidance.

## Arsenic

You might find this one interesting. The analysis behind it was
straightforward; compare maps of areas with high potential for arsenic in
groundwater to the location of all the wells, then go find the people.
Even better, it was done by one of our data MJ students here at King's, so
it is an example of something very doable by a student.
The nice thing about this story is that the analysis is beautifully simple,
yet led to a really important story. Technical complexity is not always a
prerequisite for good data journalism.
Of course, some might say a spatial join in a GIS is by definition
technically complex, but the idea, compare two layers, was elegantly
straightforward.

Here's the link: signalhfx.ca/deadly-water/

## Parking Tickets (FOIA)
One student story that worked really well and won awards was involved
getting the database of parking tickets in and around the University of
Illinois, which included Freedom of Information requests to the university
and the cities of Champaign and Urbana.
There always seems to be a good minimum story in any parking ticket
database, but in this one the student found  a few years ago that
"public agencies
are failing to collect hundreds of thousands of dollars in parking tickets in
the Champaign-Urbana area because of hurdles in keeping track of the tickets
 and pursuing parking scofflaws in the legal system."

https://dailyillini.com/local/2011/01/27/c-u-area-imposes-new-measures-after-losing-thousands-of-dollars-in-unpaid-parking-tickets/

The IRE resource center has a collection of a bunch of parking ticket
stories done around the country over the last decade.

There is a more recent story done at the University of Wyoming

https://www.ire.org/blog/extra-extra/2015/04/09/university-wyoming-experiences-sharp-rise-parking-/

One student story that worked really well and won awards was involved
getting the database of parking tickets in and around the University of
Illinois, which included Freedom of Information requests to the university
and the cities of Champaign and Urbana.
There always seems to be a good minimum story in any parking ticket
database, but in this one the student found  a few years ago that
"public agencies
are failing to collect hundreds of thousands of dollars in parking tickets in
the Champaign-Urbana area because of hurdles in keeping track of the tickets
 and pursuing parking scofflaws in the legal system."

https://dailyillini.com/local/2011/01/27/c-u-area-imposes-new-measures-after-losing-thousands-of-dollars-in-unpaid-parking-tickets/

The IRE resource center has a collection of a bunch of parking ticket
stories done around the country over the last decade.

There is a more recent story done at the University of Wyoming

https://www.ire.org/blog/extra-extra/2015/04/09/university-wyoming-experiences-sharp-rise-parking-/

## Peak Sick Days
In any large public-sector work force (teachers will do)  ask for five
years or so of sick days and see if they peak on Fridays, in such a way as
to add an extra day to holiday weekends and so forth. Interestingly Toronto
public school teachers peaked on Fridays (which we did expect) but not
Mondays (contrary to what we expected).

## Housing Inspections

Housing inspections (or inspections of any type, really) can be a great
starting place.

One that we did on Greek housing:
http://www.cu-citizenaccess.org/2013/11/20/fraternities-and-sororities-fail-inspections-violations-take-months-to-fix-2/

That story required FOIAs with Champaign and Urbana, as well. The
inspection reports actually were not housed in a database; everything was
hand-written on paper forms. I pray to the data gods that your students do
not encounter that.



---------
Dianne Finch: 

How about CO2 data from NOAA? There are many stories that could be
generated from it -- including a look at how states are taking on the Paris
agreement.....

   - NOAA


I think that global health data - or domestic health data - would be a good
choice since they have learned geospatial mapping.  Mapping diseases in
developing countries for instance --- particularly preventable diseases.

   - CDC, other gov agencies
   - World Health Organization
   - World Bank
   - Global Fund


You could give them drinking water quality data. The data could lead to
stories on government actions once lead or other toxins are found in water.


   - EPA (local and national)
   - City governments


A look at crime rates locally and nationally.  A look at prison populations
and race.
Police data in their city

All of the above had led to good stories by my students.. They start with
data and find stories.....(those who are motivated anyway!)

