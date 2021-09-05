
General description

App with server   to help strangers peoples to meat  talk and know  each other at side of meetups and other events 

#####
screens:
server:
1.create new event (header,info,location,description), generate QR
2.list of participants that made hand shake with name of the hand shakers

#####
client
1.welcome page (menu)
2.register to new event (photo QR)/by link
3.personal details (name, phone,image,details,work,linjdin,faceboook,site)
4.hand shake with other participants(by his 6 digit code) or generate my 6 digit code,can take some photo and add some comments
5.list of past events and heandshakes.
6.Optional -comunication like chat

######
Usage
HOST(server):
host instal NPM the server over Docker 
host create ne event with detail
host publish QR of the event
############
client:
download the app (or allredy has)
open the url for the new event with QR or direct link
the app get the app detail and open new event
the app send the details of the client to server
the app is generate new porsonal code and wait for hand shake(by geting other person personal code)
on hand shake, one of the sides insert other person code the app insert for both participants the event and
replace publick details , if one of then add photo it can be shared
when save, each handshaker has the info at this event list, 
afte save the creator send info to the host
history:
client can see list of old events with each events handshakes
client can see list of all handsshake contacts


#####
client android Java
applay event (barcode)




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



