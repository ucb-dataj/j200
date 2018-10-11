---
title     : Making a Map
layout    : post
category  : hands-on
tags      : [maps]
author    : Amanda Hickman
---

You should already have a [Datawrapper](https://www.datawrapper.de/) account. If you've gotten this far without creating one, we've got bigger problems.

Caroline Kee covered a pretty straightforward, if disturbing, CDC report on [rising suicide rates nationwide](https://www.buzzfeed.com/carolinekee/suicide-rates-increase-us-2016-all-states). The map she included came directly from the CDC. It isn't a terrible map, but there are a few ways it could be much better. Can you tell at a glance **which states stand out** as having the most severe increase?

Take a look at the legend. The sizes on those buckets are wild. The darkest has a 20 percentage pt spread, and the next has just a six percentage pt spread. These are quantiles: the CDC designed the buckets so that each would have 12 states in it. And then they chipped off Nevada which is the only state that saw a decrease.

Luckily, BuzzFeed News actually links to the original report -- the raw data is available in the CDC's [original report](https://www.cdc.gov/vitalsigns/suicide/infographic.html#graphic1) which appeared in the [Morbidity and Mortality Weekly Report](https://www.cdc.gov/mmwr/index.html). To avoid hiccups in the copy and paste process, I went ahead and pulled the numbers for you.

<https://app.workbenchdata.com/workflows/5852>

Workbench is still a work in progress but one thing it does well is show the transformations I applied to the original data.

**Step 0:** Download the csv from Workbench.

**Step 1:** Log into Datawrapper and choose "Create a map". We want a choropleth.

![create a map](/j200/assets/mapping_exercise/dw1.png)

**Step 2:** (Datawrapper thinks of this as Step 1), search for "USA States" under "What type of map do you want to create?".

**Step 3:** Import your dataset. But get in the habit of reading pop up windows. Do we have ISO-Codes or Names here?

Once you've uploaded your data, read through the next screen, too.

![pay attention](/j200/assets/mapping_exercise/columns.png)

As you step through these dialog windows, they should make sense!

You've already got a much cleaner map. But we're going to hit `Proceed` and make it better.

**Step 4:** Customize your gradient and your tooltips. The average nationwide was a 25.4% increase. You could reasonably center your buckets there. Or you can keep the default gradient. And make some tooltips.

```
\{\{ Increase_Decrease }} of {{ Overall_Percent_Change }}%
```

**Step 5:** Add your title and description. Never skip the metadata.

**Title:** What is the takeaway here? In the story, they captioned this "Suicide rates increased in almost all states between 1999 and 2016 — some by more than 30%.", but the chart uses "Figure. Percent change in annual suicide rate,* by state-- United States , from 1999/2001 to 2014/2016"

**Caption:** Tell your readers more about what we're looking at. "A recent CDC report found that there is just one state in the union -- Nevada -- where suicides did  not rise between 1999 and 2016."

**Step 6:** Embed it!


## Unsolved Homicides

The Washington Post collected data on more than 52,000 criminal homicides over the past decade in 50 of the largest American cities. I filtered out two local cities so we could take a closer look.
[Unsolved Homicides in Oakland](https://app.workbenchdata.com/workflows/5840) \ [Unsolved Homicides in San Francisco](https://app.workbenchdata.com/workflows/5853/). We could map these in Datawrapper but we're going to get frustrated with their built in maps.

Another excellent option if you're willing to learn (or cut and paste) some javascript is Mapbox Studio.

0. Download the unsolved homicides CSV that you're interested in. Make sure you know where your computer stored it.
1. Make an account.
2. Head into [Mapbox Studio](https://www.mapbox.com/studio/) once you're logged in.
3. On the "Datasets" tab, click on "New dataset" -- upload your csv.

You can very quickly start looking at the data on a map. We can also go back to the Studio menu and start to work on making styles. Mapbox likes to start in Paris. If you aren't making a map of Paris search for a different city so you can center your map there.

Add a layer. Even though you already uploaded it, you want to select "upload" and then look for Create From Dataset.
