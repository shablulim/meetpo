
General description

help strangers peoples to meat  talk and know  each other at side of meetups and other events 

#####
screens
Host-
registration & login
details
events list
event- crude
participents-crude
register participants to event
event summery(includes mutches)
cpmunicate sutch emails etc after events

#####
client (react hook, no redux, but only  recoiljs  or context, maybe typescript)
registration
applay event (barcode)
personal data
handshake other participants & handeling(comments, selfy)
events history
chat with others from handshake








####
server (node express on Ubuntu)


####
database(mongo or mySql)

collections:


participents
id:"",
personal info:{
   name,address,phone,fb,linkedin etc
},
events_attends:[
   {event_id:"",
    hand_shake:[{participent_id:"",
                 comment:"",
                 photoes:[link,link]
                 }]
   },
      {event_id:"",
    hand_shake:[{participent_id:"",
                 comment:"",
                 photoes:[link,link]
                 }]
   },  {event_id:"",
    hand_shake:[{participent_id:"",
                 comment:"",
                 photoes:[link,link]
                 }]
   },
    
]


events
id:"",
name:"",
date:"",
place:"",
header:"",
comment:"",
total_registers:"",
attended:[
   {participant_id:"",hand_shakes:""},
   {participant_id:"",hand_shakes:""},
   {participant_id:"",hand_shakes:""},
   {participant_id:"",hand_shakes:""}
]



