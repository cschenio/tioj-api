tioj-api
========
The API rules for open source online judge -- TIOJ.

TIOJ
----
TIOJ was named Temporary INFOR Online Judge, which is the online judge platform for a high school club INFOR whose member are interested in the informatic field from 00s to 2013.
Since the judge remained 'temporary' for years, the abbreviation TIOJ for the corresponding whole name was common among informatic-interested students in Taiwan. Therefore, after we rebuilt it in 2014, we decided to name it TIOJ INFOR Online Judge, which the first word is the recursive acronym.

API
---
We firstly programmed the [new platform](https://github.com/joshua5201/tioj) in Ruby on Rails. But in 2016, one of our members [Yi-yo Chiang](https://github.com/silverneko) decided to port it to Golang, called [GIOJ](https://github.com/silverneko/gioj). It made me think of designing an API for TIOJ, which any client-side with any server-side architecture can plug-and-play with each other well whatever the languages are. 

Reference
---------
### Related repository
+ [TIOJ](https://github.com/joshua5201/tioj)
+ [GIOJ](https://github.com/silverneko/gioj)