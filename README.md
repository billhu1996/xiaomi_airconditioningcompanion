# Xiaomi Mi and Aqara Air Conditioning Companion

This is a custom component for home assistant to integrate the Xiaomi Mi and Aqara Air Conditioning Companion (KTBL01LM, KTBL02LM).

Please follow the instructions on [Retrieving the Access Token](https://home-assistant.io/components/xiaomi/#retrieving-the-access-token) to get the API token to use in the configuration.yaml file.

Credits: Thanks to [Rytilahti](https://github.com/rytilahti/python-miio) for all the work.

## Features
* On, Off
* Operation Mode
* Temperature
* Speed
* Swing Mode
* Fan Mode

## Setup

```yaml
# confugration.yaml

climate
  - platform: xiaomi_miio
    name: Aqara Air Conditioning Companion
    host: 192.168.130.71
    token: b7c4a758c251955d2c24b1d9e41ce47d
    target_sensor: sensor.temperature_158d0001f53706
    scan_interval: 60
    customize:
      swing:
        top: 010501820000261801
        down: FEADASDSDSDSDSDSADSAFADSFASA
      fan:
        max: FEADASDSDSDSDSDSADSAFADSFASAD
        med: FEBDASDSDSDSDSDSADSAFADSFASAR
        min: 010501A20000261B01
```
