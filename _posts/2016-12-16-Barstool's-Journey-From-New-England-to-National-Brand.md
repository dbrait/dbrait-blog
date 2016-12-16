---
title: "Barstool's Journey From New England to National Brand"
author: "David Brait"
date: "Friday, December 16, 2016"
output: 
  html_document:
    code_folding: hide
---

```{r global_options, include=FALSE}
library(knitr)
```

As someone who became a stoolie in 2014, watching the progression of Barstool from a regional brand into a national one has been fascinating.  At this point if you are of a certain age you have likely heard of Barstool in some capacity, whether you it's "Saturday's Are For the Boys" or "Pardon My Take", there are several facets of the brand that have resonated and spread on a national scale.

If you are of a certian age in New England, Barstool has likely driven the sports and pop culture conversation, more so than NESN, Felger and Mazz or the Boston Globe.  Many have speculated that El Pres is the most powerful person in Boston sports media.

What anybody who even casually follows understands is the way in which Barstool resonates with it's readers.  In an era where trust in media is at an all time low and many of the new media models focus first on technology and virality, barstool goes against the grain.  It's tech until recently was at best a detriment and probably better described as a disaster.  Any reader understands that the site's personalities are authentic and honest, they speak to many issues that are outside the realm of a sports media complex that is increasingly hollow and out of touch.

Sites that have large venture capital funding have focused on the distribution almost at the expense of the product.  

I had a pretty good grasp for how the data might look.  I decided to look at the last five years of facebook data.  The data dates back to 2013 (when barstool really started to become active on facebook).  For any modern media company Facebook has become the lifeblood with its ability to make content go viral. 

When you break down the year by year data, the obvious impact of Chernin is remarkable.  You can see that barstool became cognizant of the need for a facebook strategy, in particular last year (2015) with the number of posts seeing a huge uptick:

<img src="img/num_posts_year.png">

But in terms of virality and distribution they had stagnated in the same place for the last three years.  2016 saw an enormous uptick in their consistent ability to spread content:

<img src="img/avg_shares_year.png">
<img src="img/med_shares_year.png">

The data is so varied and seemingly random in some spots, so it helps to understand barstool.  Each of the spikes until mid 2015 has a New England based explanation.  

The Boston Marathon stories of resilience of victims and first responders generated huge bumps in 2013 during the bombings.  It was the first major leap barstool made as they maintained many of their numbers througout the year.  It was also a great leading indicator of the power of their engagement.  For a cause in their wheelhouse they were able to generate an enormous amount of traffic and turn it into something tangible.

<img src="img/avg_shares_2013.png">

```{r, echo=FALSE}
top_posts_2013 <- read.csv("data/top_posts.csv")
top_posts_2013 <- top_posts %>% filter(Year == 2013) %>% head(top_posts_2013, 10)
kable(top_posts_2013)
```

and again in 2014 covering the one year anniversary. 

<img src="img/avg_shares_2014.png">

```{r, echo=FALSE}
top_posts_2014 <- read.csv("data/top_posts.csv")
top_posts_2014 <- top_posts_2014 %>% filter(Year == 2014) %>% head(top_posts_2014, 10)
kable(top_posts_2014)
```

The various inflection points of deflategate and the sit in at NFL headquarters generated in early 2015.

<img src="img/avg_shares_2015.png">

```{r, echo=FALSE}
top_posts_2015 <- read.csv("data/top_posts.csv")
top_posts_2015 <- top_posts_2015 %>% filter(Year == 2015) %>% head(top_posts_2015, 10)
kable(top_posts_2015)
```

In late 2015 there is a big jump around November as the number of shares rose to 90-100 per post and the average likes climbed to 300.  Barstool has maintained this level for the past year.

You can also see Barstool start to make a transition.  Of the 20 most shared posts in 2015, 16 of them came after September 1st.  The jump in numbers is staggering towards the end of the year, with the kill everybody tour and fire goodell content still the main source of shares, but with a combo of more clickbaity content and some organic barstool content mixed in (most notable the big cat Detroit Don video which did an enormous 35,127 shares)

The move to the New York office shows promising signs of being a big content generator as 9 of 2016's top 10 posts are from September or October.  Barstool has always had the ability to make something go viral and general 10,000+ shares, usually with stories that unite New England in a big way.  What has shifted in the last year is their ability to constantly drive number of shares for a wide variety of content on a regular basis.  If early indicators hold true, it looks like they have made another major leap since the birth of the new office.  2016 is the first year where New England has not dominated the top content.  All five top posts this year are non New England stories.

```{r, echo=FALSE}
top_posts_2016 <- read.csv("data/top_posts.csv")
top_posts_2016 <- top_posts_2016 %>% filter(Year == 2016) %>% head(top_posts_2016, 10)
kable(top_posts_2016)
```

&nbsp;

{% include twitter_plug.html %}
