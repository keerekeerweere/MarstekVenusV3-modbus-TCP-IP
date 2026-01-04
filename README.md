# MarstekVenusV3-modbus-TCP-IP
### **Home assistant yaml files to readout the Marstek V3 directly through ethernet by modbus TCP-IP**

* To use this in your Home Assistant setup add this block to your main configuration.yaml file:
```
homeassistant:
  packages: !include_dir_named packages
```
* Create a subfolder called packages and copy the "marstek_m1_modbus_tcp.yaml" file from this repo to the folder => /config/packages/marstek_m1_modbus_tcp.yaml
Change [IPADRESS] in the yaml to your own marstek battery IP adress.

* Restart your Home Assistant.

* You can add the code of the MENU yaml file to your home assistant.
In home assistant choose the pencil in the upper right corner.
Press + on the top menu. Choose building blocks (bouwstenen) and save (opslaan)
Choose pencil and three dots - edit in yaml (bewerken in yaml) en copy all the code from inside the marstek_m1_modbus_tcp_MENU.yaml file to this screen and click save
The entities created from marstek_m1_modbus_tcp.yaml should now be available.
For the graphics inside the menu go to HACS (if installed) and install apexcharts-card

* For more batterys then one - use upfollowing yaml files (m2 - m3 - m4)
