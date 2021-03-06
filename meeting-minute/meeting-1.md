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
* create mapping between team and match

#Note for everyone
1. Communicate with each other whenever necessary (UI or backend)
1. Discussion can be made on mailing list
