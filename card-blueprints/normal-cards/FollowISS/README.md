# FollowISS Blueprint

- This blueprint can be used as a card or as a pop-up.

## Installation of this Blueprint

- Install vertical-stack-in-card from [HACS]

- Add the following sensor in the configuration.yaml or sensors.yaml file. The sensor is used to extract the states of the ISS. 

# ISS Sensors
          
  - platform: template
    sensors:
      international_space_station_peoples_in:
        friendly_name: "Iss Peoples"
        icon_template: mdi:account-group
        value_template: "{{ state_attr('binary_sensor.iss', 'number_of_people_in_space' ) }}"
        
  - platform: template
    sensors:
      international_space_station_next_rise:
        friendly_name: "Iss next rise"
        icon_template: mdi:waves-arrow-up
        value_template: "{{ state_attr('binary_sensor.iss', 'next_rise' ) }}"
        
  - platform: template
    sensors:
      international_space_station_longitude:
        friendly_name: "Iss longitude"
        icon_template: mdi:longitude
        value_template: "{{ state_attr('binary_sensor.iss', 'longitude' ) }}"
        
  - platform: template
    sensors:
      international_space_station_latitude:
        friendly_name: "Iss latitude"
        icon_template: mdi:latitude
        value_template: "{{ state_attr('binary_sensor.iss', 'latitude' ) }}"


- Restart Home Assistant

Make sure you have following installed this can be done manually or directly via hacs
- Cards
    - [state-switch](https://my.home-assistant.io/redirect/config_flow_start?domain=iss)

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for each card.

 - Translate Number of people on board in your language
 - Translate next rise in your language
 - Translate longitude in your language
 - Translate latitude in your language
 - Disable dark mode for map

### Screenshots
**Light theme:**<br>

**Card**

**Dark theme:**<br>


### Changelog
#### 1.0
- First release
