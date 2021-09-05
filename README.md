
General description

help strangers peoples to meat  talk and know  each other at side of meetups and other events 

#####
screens:
server:
1.create new event (header,info,location,description), generate QR
2.list of participants that made hand shake with name of the hand shakers

client
1.welcome page (menu)
2.register to new event (photo QR)/by link
3.personal details (name, phone,image,details,work,linjdin,faceboook,site)
4.hand shake with other participants(by his 6 digit code) or generate my 6 digit code,can take some photo and add some comments
5.list of past events and heandshakes.
6.Optional -comunication like chat

Host-


#####
client (react hook, no redux, but only  recoiljs  or context, maybe typescript)
registration
applay event (barcode)
personal data
handshake other participants & handeling(comments, selfy)
events history
chat with others from handshake








####
server (node express on Ubuntu)/DOCKER


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



