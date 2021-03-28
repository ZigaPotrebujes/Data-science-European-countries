# Data science starter pack

Let me start by explaining what the _real_ purpose of this analysis is. At my previous employment, I learned that one of the things you use most (as a data scientist at least) is Copy-Paste. There are a finite number of plots and infinite number of problems. Things are bound to repeat themselves, but that is a good thing! I learned that people (especially coworkers from other fields) quickly tend to lose interest if there is too many new things going on. A new color or some other feautre here and there is fine, but don't overdo it. That's why some degree of repetitiveness in this line of work is a must and I wanted to create a project where I would have different plots and its code, so I can always easily find it. Therefore, since the actual content is more of a secondary nature in this post, you may find it more interesting from a technical point of view. In this document I will stick more to my thought process, while the code itself will be stored in the workspace file. 

In short:
**Objectives**
- create a short analysis, containing few charts, which will help with copy pasting me in the future
- extract at least 1 piece of useful information (to me) in the process

I started searching for a dataset on [Kaggle](https://www.kaggle.com/). I found one that interested me about quality of life in Europe. I went straight to the source and scraped the data. 

## Cost of living
**SOURCE:** https://www.numbeo.com/quality-of-life/rankings_by_country.jsp?title=2021

* extracted data from the source for different years
* map plot of quality of life (on first glance looks OK)

![alt text](https://github.com/ZigaPotrebujes/Data-science-starter-pack/blob/main/plots/DS1-QoL-facet.png)

* did the same thing for 2 more metrics - healthcare and safety

![alt text](https://github.com/ZigaPotrebujes/Data-science-starter-pack/blob/main/plots/DS1-hc-facet.png)
![alt text](https://github.com/ZigaPotrebujes/Data-science-starter-pack/blob/main/plots/DS1-safety-facet-num.png)

* the latter triggered an alarm in my head. Sweden was far too gray for my opinion and I wanted to double check that
* first thing I did was present the data in a different way so that the actual safety score is a bit clearer

![alt text](https://github.com/ZigaPotrebujes/Data-science-starter-pack/blob/main/plots/DS1-safety-barpl-numbeo.png)

* my fears were confirmed. I **sincerely** doubt Sweden is more dangerous than Ukraine which had seen war in the recent years and hostilities still haven't really ended
* it even popped up in the top 10 most dangereous countries _worldwide_
* Upon checkin reviews I noticed other people had similar problems with Numbeo, especially with the crime scores. Although it is a hard metric to quantify, the current method they use is to survey users, which is far from reliable source of data
* I also decided to look for other sources. The first one is [Eurostat](https://ec.europa.eu/eurostat/statistics-explained/index.php?title=Archive:Quality_of_life_in_Europe_-_facts_and_views_-_economic_and_physical_safety&oldid=400085#Data_sources_and_availability), which is a credible source of information. It already had the data neatly prepared in charts, for our convenience. 


#<img src="https://github.com/ZigaPotrebujes/Data-science-starter-pack/blob/main/plots/DS1%20-%20CLI-2020.png" width="750" height="600">
