# Methodology Notes 

`Weather` = wind and air monitor
`Atlas` = ph, orp, temp, ec, do monitor
`Sonar` = depth sensor

### Preparation

##### Calibration

- clean flux from female header pin solder for Atlas sensors using rubbing alcohol + toothbrush
- connect calibration feather to Atlas PCB 
- connect to device using `screen /dev/tty.usbmodemXXXX 115200`
- run `ph`, `orp`, `do`, `ec` – follow directions in Atlas pdf documents and refer to notes in calibration 

##### Assembly

All systems: 

- Attach battery pack to the PCB 

Weather: 

- Attach mounting bracket to the back of each weather station (reapply silicon on screws)

Atlas: 

- run probe cables, temperature sensor cable, and power cable through the gland opening 
- insert rubber hose piece into the gland opening around the cables, seal with silicon.

Sonar: 

- (in some cases) attach back bracket to the device

##### Testing system

- Connect battery to Weather
- wait for preflight to run success if three fast blinks, if slower blinks then look at memory card for debugging logs 
- If Weather is successful, connect power to Atlas and Sonar and then  after enough time for systems to power on, connect power to Weather 
- Wait for systems to talk to eachother, then look at Weather memory card for debug logs 

Things to look for:

- system is able to connect to GPS
- able to uplink via satellite
- LORA communication works between water sensors and Weather

### Deployment

supplies to bring: 

- hose clamp
- three modules which have been tested and calibrated
- tripod (and pikes)
- weather station hardware 
- stake for the water sensors 
- mallet for planting stake
- device for measuring GPS position 
- wrench for hose clamps 
- photographer (optional) 


collecting old monitor (only at certain stations):

- take photos of current state of the station (surroundings and electronics)
- break down the system 
- if weather monitoring hardware is operational, leave it in place

deploying station: 

- set up tripod with weather station hardware
- attach Weather system to tripod, solar panel pointed towards the sun 
- plant water sensor stake into the water nearby the tripod
- attach Atlas and Sonar to the stake (position two on each stake, solar panel pointed towards the sun. Prioritize more power for the Atlas)
- connect power to each module 

post deployment: 

- take photos of area where each sensor is 
- record GPS coordinates for position of each sensor

### Confirmation

- we need to confirm sensor is working when it is out in the field
- TODO: get more details on this 




