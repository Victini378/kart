# KART (Kafka Automatic Referral Triage)
![](https://mario.wiki.gallery/images/thumb/a/a0/MK8_Mario_Drifting_Standard_Kart_Shadowless_Artwork.png/200px-MK8_Mario_Drifting_Standard_Kart_Shadowless_Artwork.png)

## Description 

Mario is an healthcare professional working at the Nintendo Cars Garage, 
where players go if they have incidents during the the races.
Every car has a "black box" containing a log in text format with recents events.
The last line has a special code defining the status of the car.
Mario would like to dispatch automatically the cars according to the level of damage indicated in the status in two queues:
- recoverable: cars that can be repaired 
- scrap: cars that need to be demolished

## Challenge
Help Mario implementing a system based of files put in a given directory 
(choose the format, remember to be able to distinguish the status in the last line)
send to Kafka and using Kafka Stream perform a triage and sent to the appropriate topic
Use kafka consumer to show the status of the queues
