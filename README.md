# HA-OS Gree Climate
# HA Gree climate as custom integration that work from another LAN segment, you can specify AC IP address.
# Done because HA team decided not to update the official Gree integration to work from any LAN segment.

1. copy all from Gree to custom_components/gree/<br>
2. restart HA<br>
3. check log for errors<br>
4. If no errors then go to Integration - Add integration - Gree Climate and enter AC IP if it is not found automaticaly.<br>
   
5. If AC it is find and set-up OK check your Gree Climate - Integration entries and rename switches if required, you can find the switch name in core.entity_registry:<br>
     "entity_id": "switch.MAC_none"    ->  Panel Light<br>
     "entity_id": "switch.MAC_none_2"  ->  Quiet<br>
     "entity_id": "switch.MAC_none_3"  ->  Fresh Air<br>
     "entity_id": "switch.MAC_none_4"  ->  XFan<br>
     "entity_id": "switch.MAC_none_5"  ->  Health mode<br>

DONE<br>
<br>
This integration it is made from original HA OS Gree Climate Integration and patch from kspearrin:<br>
<br>
https://github.com/home-assistant/core/pull/100731<br>
https://github.com/home-assistant/core/tree/ec2116a3e78efe9bcbb35434efc6c84d568a6eba/homeassistant/components/gree<br>
https://github.com/home-assistant/core/tree/ec2116a3e78efe9bcbb35434efc6c84d568a6eba/tests/components/gree<br>

![gree-1](https://github.com/rapi3/HA-OS-Gree/assets/18531150/9ff6e997-ad80-4298-ac90-dda103422f0d)
