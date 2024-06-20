# HA-OS Gree
# Gree climate custom integration that work from another LAN segment, you can specify AC IP address.

1. copy all from Gree to custom_components/gree/
2. restart HA
3. check log for errors
4. If no errors then go to Integration - Add integration - Gree Climate and enter AC IP if it is not find automaticaly.
   
5. If AC it is find and set-up OK check your Gree Climate - Integration entries and rename if required switches, you can find the switch name in core.entity_registry:
     "entity_id": "switch.MAC_none"    ->  Panel Light
     "entity_id": "switch.MAC_none_2"  ->  Quiet
     "entity_id": "switch.MAC_none_3"  ->  Fresh Air
     "entity_id": "switch.MAC_none_4"  ->  XFan
     "entity_id": "switch.MAC_none_5"  ->  Health mode

DONE

This integration it is made from original HA OS gree climate integration and patch from kspearrin:

https://github.com/home-assistant/core/pull/100731
https://github.com/home-assistant/core/tree/ec2116a3e78efe9bcbb35434efc6c84d568a6eba/homeassistant/components/gree
https://github.com/home-assistant/core/tree/ec2116a3e78efe9bcbb35434efc6c84d568a6eba/tests/components/gree
