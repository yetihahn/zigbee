---
model: XHS2-UE
vendor: UEI
title: Comcast Xfinity Door/Window Sensor
category: sensor
supports: contact, temperature, battery
zigbeemodel: ['URC4460BC0-X-R']
compatible: [z2m]
mlink: 
link: https://www.amazon.com/Zigbee-Sensors-XHS2-TY-XHS2-UE-Security/dp/B01N3CVD4L
link2: 
link3: 
---
19 April 2022 - was able to connect and see some states (open/close and temp, NOT battery level) change using Sonoff Zigbee Bridge flashed with Tasmota via ZHA. Was also able to connect with a Conbee II via ZHA, however, states were not updated and the divice was not recoginzed by ZHA (calling the unit "unk_manufacturer unk_model") YMMV.

To pair a new unit: remove the plastic battery tab on the back. LED will flash showing the unit is in pairing mode. If the unit doesn't pair to a network within 100 sec the unit will go to sleep. To wake the unit up, place the magnetic contact sensor near the unit. You can appatently also touch the tamper swtich. I have not tried this though. 

To creat a "new pairing" (moving from one coordinator to another) you need to reset the unit (remove case, remove battery, wait 5 sec, hold tamper button for 3 sec, reinsert the battery, when the LED turns on release the tamper button {waiting too long to release the tamper switch will cause the LED to light up, blink SUPER fast, then turn off without pairing}) and it should go into pairing mode. 
