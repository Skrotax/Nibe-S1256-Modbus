Just how i set up my Nibe S1256 heatpump.

Check https://github.com/elupus/esphome-nibe 
and 
https://www.home-assistant.io/integrations/nibe_heatpump

I did not like the +700 unused entities that the integrated Nibe produces. 

Exported the modbus list from my heatpump at set the sensors i am interested in manually, I.E, i used mkaiser´s modbus_sungrow.yaml as a template. 

https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant

Made 4x input numbers from UI, see input.numbers.txt

Corresponding automations also as .txt files and can be directly pasted into the UI yaml editor.

My heat pump dashboard.yaml and .png file also attached. (picture element)

Hope it helps someone

br. /JR
