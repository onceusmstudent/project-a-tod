##Objective
1. To learn UI design (Data visualization)
1. To learn proper system design and architecture
1. To learn proper SDLC

---
##Functional Requirement
1. Historical data visualization of Dota2 tournament winning rate
  * date range
  * version
  * team A
  * team B
2. Team stats
3. Match stats
4. User account management (user-specific content)
5. In site search feature

---
##Non-functional Requirement
1. Compute intensive
2. Responsive UI
3. Modern browser support
  * Chrome
  * Firefox
  * Safari
  * Opera
1. Data-centric [IO-bound]

---
##Technology choices
Database: [MongoDB](https://www.mongodb.org/)

Backend Language: [Scala](http://www.scala-lang.org/)

Web Framework: [Play 2.0](https://www.playframework.com/)

Frontend visualization:
* [Angular.js](https://angularjs.org/)
* [Highcharts.js](http://www.highcharts.com/)
* [Bootstrap](http://getbootstrap.com/)

---
##Backend Requirement
* retrieve data from [steam API](http://dev.dota2.com/showthread.php?t=47115)
* CRUD with MongoDB
* Local data has higher priority over external data, external data act as a fallback of local data


##Miscellaneous
* Testing : [ScalaTest](http://www.scalatest.org/)
* Bug Tracking : Github issue tracking
* Coding Convention : [Scala default](http://docs.scala-lang.org/style/)
* Documentation : whenever necessary
* VCS : [Git branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

##WebAPI details
[WebAPI Documentation](https://wiki.teamfortress.com/wiki/WebAPI)

ps: Team is not associated with match

##User-stories
### Main Page<a name="usercase1"></a>
1. Responsive design
1. Provide summary of all feature (based on what we have right now)
1. Show upcoming match in time line graph, where points on the graph should be interactive and can provide more information when hover/clicked

###Historical win loss visualization
1. show historical data of team A vs team B
1. show historical data of team A vs all

###Team stats summary
1. win lose
1. top pick hero

###Match stats summary
1. top kill, top farm etc
1. most unpeaceful period
1. hero kill/death trend through out game
1. tower kill/death trend etc

##Distribution of work
###Yih Yew (Lead Web Designer)
* create Main Page
* define a base look and feel style for other to follow

###Kelvin (Lead Backend Developer)
* handle backend data management
* the only person with direct db access
* provide data service to other module
* note: disk access should be asynchronous and non-blocking

###Han Lin
* create Team stats summary and match stats summary

###Chen Wai
* create Historical win loss visualization

###Qing Wei
* provide service to query team and match

#Note for everyone
1. Communicate with each other whenever necessary (UI or backend)
1. Discussion can be made on mailing list
1. All data are provided by Kelvin, do not attempt to fetch from api or db
