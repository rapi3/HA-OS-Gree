HA-OS Gree Climate<br>
HA Gree climate as custom integration that work from another LAN segment, you can specify AC IP address.<br>
Done because HA team decided not to update the official Gree integration to work from any LAN segment.<br>
HACS installation:<br>
<br>
Go to Home Assistant and navigate to HACS.<br>
In HACS, select "Integrations".<br>
Click on the three dots button in the upper right corner and select "Custom repositories".<br>
In the window that appears, enter the URL of this repository https://github.com/rapi3/HA-OS-Gree and select the category (Integration).<br>
Click on "Add".<br>
Manual instalation:<br>
<br>
copy all from gree to custom_components/gree/<br>
restart HA<br>
check log for errors<br>
Set-up:<br>
If no errors then go to Integration - Add integration - Gree Climate and enter AC IP if it is not found automaticaly.<br>
<br>
If AC it is find and set-up OK check your Gree Climate - Integration entries and rename switches if required, you can find the switch name in core.entity_registry:<br>
"entity_id": "switch.MAC_none" -> Panel Light<br>
"entity_id": "switch.MAC_none_2" -> Quiet<br>
"entity_id": "switch.MAC_none_3" -> Fresh Air<br>
"entity_id": "switch.MAC_none_4" -> XFan<br>
"entity_id": "switch.MAC_none_5" -> Health mode<br>
<br>
DONE<br>
