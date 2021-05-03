# ESPhome-irrigation


 
 Forked from: https://github.com/brianhanifin/esphome-config

In the fact, this is https://github.com/brianhanifin/esphome-config code 
with some changes: other board, add water pump control, add virtual switch
to suspend whole automation, which could be maintained with HA.

Lovelace entry explained in original post here: 
https://brianhanifin.com/posts/diy-irrigation-controller-lovelace-ui-update/

Reworked with great help from ESPhome discord : https://discord.gg/fTTT6eAwpF

Whole automation is controlled by ESPboard, settings through HA cards. 
In case of lost connection with HA automation still works, 
and resets itself 'automation suspend' every 2 days .

-Todo: connect somehow 'automation suspend' with some web weather service-

2 relays for valves, one for water pump (switch off is delayed, lets the pump 
rebuild pressure). One relay is spare so far.
~~PCB has 5V voltage regulator (Vin up to 35V) build under NodeMcu board~~,

 and relays are controlled via transistors. It has possibility to control it 
through switches connected to gpio. Maybe I 'll add radio control with 
4button remote, but I don't know if esp8256 can handle it, maybe I'll switch
 to esp32

 
