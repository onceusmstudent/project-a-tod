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

##Program Structure
> to be discussed

##Miscellaneous
* Testing : [ScalaTest](http://www.scalatest.org/)
* Bug Tracking : Github issue tracking
* Coding Convention : [Scala default](http://docs.scala-lang.org/style/)
* Documentation : whenever necessary
* VCS : [Git branch workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

#To do
* find out what is provided by Steam Dota 2 Api
* check on Scala
