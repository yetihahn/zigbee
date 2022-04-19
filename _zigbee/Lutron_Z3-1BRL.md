---
date_added: 2020-02-15
model: Z3-1BRL
vendor: Lutron
title: Aurora Smart Bulb Dimmer
category: remote
supports: action, brightness
image: /assets/images/devices/Lutron_Z3-1BRL.jpg
zigbeemodel: ['Z3-1BRL']
compatible: [z2m,zha,deconz]
deconz: 2305
mlink: http://www.lutron.com/en-US/pages/SupportCenter/support.aspx?productName=Aurora%20smart%20bulb%20dimmer&SECTION=Documents
link: https://www.amazon.com/Lutron-Aurora-Dimmer-Philips-Z3-1BRL-WH-L0/dp/B07RJ14FBS
link2: 
link3: 
---

19 April 2022 - was able to pair unit to Sonoff Bridge flashed with Tasmota via ZHA. As well as a Conbee II via ZHA. The button press worked much better with Conbee II (though I was also testing using the Blueprint mentioned below with the Conbee and solely NodeRed with the Sonoff Bridge.) When using the Sonoff (and no Blueprint) the button would change values (from 0 to 255) but wouldn't update untill the knob was slightly turned (now showing 254).

To get unit into pairing mode: quickly tap the front button twice. A blinking light will indicate it is in pairing mode. 

To factory reset the unit: quickly tap the front button three times, holding the button down on the third press. Wait for the LED to start flashing quickly, then quickly tap the front button three more times. The unit should then be reset. 

If using in Home Assistant I HIGHLY recommend using this BluePrint: https://community.home-assistant.io/t/zha-lutron-aurora-dimmer-blueprint/292421 It worked much better (and faster) than NodeRed to convert the ZHA_events into usable actions when I was testing it. 
