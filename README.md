# HomeAssistant_Platforms
Contain new created or edited platform based on default platform of home assistant open source.

# How to apply Platform:
- Download target .py file
- Add downloaded files to home assistant install directory. Exanple:/srv/homeassistant/lib/python3.4/site-packages/homeassistant/components
- Restart home Assistant.
- DONE

# List of Platform:

- heatpumpsepo.py
  - What difference? 
    - Default heatpump does not support MQTT protocol
    - Adding publish message with pay_load in JSON: CONTROLLAC {\"ID\":\"%s\",\"State\":\"ON\",\"mode\":\"%s\",\"temp\":\"%d\",\"fan\":\"%s\",\"swing\":\"%s\"}"
    - Change more practical config for AC:
      - Mode: Cool/Dry/FanOnly/Auto
      - Narrow temperature: 18-30 C degree
      - Fan Mode: Max/Med/Min/Auto
      - Swing Mode: ON/OFF
