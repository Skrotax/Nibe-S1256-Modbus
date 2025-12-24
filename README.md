Just how i set up my Nibe S1256 heatpump.
https://github.com/Skrotax/Nibe-S1256-Modbus/blob/main/dashb_VP_show.png


Check https://github.com/elupus/esphome-nibe 
and 
https://www.home-assistant.io/integrations/nibe_heatpump

I did not like the +700 unused entities that the integrated Nibe produces. 

Exported the modbus list from my heatpump at set the sensors i am interested in manually, I.E, i used mkaiser´s modbus_sungrow.yaml as a template. 

https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant



copy modbus_nibes1256.yaml to config\integrations directory


Made 4x input numbers from UI, see input.numbers.txt

Corresponding automations also as .txt files.

Automation___.txt files can be directly pasted into UI


My heat pump dashboard.yaml and .png file also attached. (picture element)

vp_dashboard.yaml. can be pasted into dashboard raw editor

copy vp_v2_mg.png to config\www directory




Hope it helps someone

br. /JR
