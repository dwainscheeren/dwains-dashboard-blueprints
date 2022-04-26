# FollowISS Blueprint

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

Make sure you have following integration installed.

- [ISS](https://www.home-assistant.io/integrations/iss/)

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for each card.

 - Translate Number of people on board in your language
 - Translate next rise in your language
 - Translate longitude in your language
 - Translate latitude in your language
 - Disable dark mode for map

### Screenshots
**Light theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/165318714-ada4cc7e-9183-40a0-8f8b-570ee9130c78.jpeg)

**Dark theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/165318746-d53bf531-58ab-4330-8235-f88cefb38f14.jpeg)

### Changelog
#### 1.0
- First release
