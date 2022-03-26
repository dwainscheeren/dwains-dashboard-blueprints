# SunMoonSeason Blueprint

## Installation of this Blueprint

- Install compass-card from [HACS]
- Install sun-card from [HACS]

- This card needs the following three integrations to work.

##Sun

    This integration is by default enabled, unless you’ve disabled or removed the default_config: line from your configuration. If that is the case, the following example shows you how to enable this integration manually:

  # Example configuration.yaml entry

    sun:

##Moon

    To enable the moon sensor, add the following lines to your configuration.yaml or your sensors file:

  # Example configuration.yaml entry

    sensor:
       - platform: moon

##Season

    To enable the season sensor, add the following lines to your configuration.yaml or your sensors file:

  # Example configuration.yaml entry

    sensor:
       - platform: season

 # For the Sun and Compass cards, you need to add the following sensors lines to your configuration.yaml or your sensors file:

sensor:
  - platform: sun2
    entity_namespace: sun2
    monitored_conditions:
      - solar_midnight
      - astronomical_dawn
      - dawn
      - solar_noon
      - dusk
      - astronomical_dusk
      - daylight
      - civil_daylight
      - astronomical_daylight
      - night
      - civil_night
      - astronomical_night
      - elevation
      - min_elevation
      - max_elevation
 
  - platform: sun2
    entity_namespace: sun2
    latitude: xx.xxxxxxxx     # Your latitude
    longitude: -xx.xxxxxxx    # Your longitude
    time_zone: time zone      # https://en.wikipedia.org/wiki/List_of_tz_database_time_zones
    elevation: 116
    monitored_conditions:
      - sunrise
      - sunset

# Elevation
  - platform: template
    sensors:
      solar_angle:
        friendly_name: "Altitude"
        unit_of_measurement: "°"
        value_template: "{{ state_attr('sun.sun', 'elevation') }}"
        
# Azimut
  - platform: template
    sensors:
      solar_azimut:
        friendly_name: "Azimut"
        unit_of_measurement: "°"
        value_template: "{{ state_attr('sun.sun', 'azimuth') }}"
      
binary_sensor:
  - platform: sun2
    entity_namespace: sun2
    monitored_conditions:
      - elevation
      - elevation: 3
      - elevation:
          above: -6
          name: "Above the civil dawn"

# Sun image for compass

- Copy the Sun image in /config/www/images. Note: This image can be anything you want, but it must have the name Sun.png

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for each card.

 - Translate Sun in your language   EX : Soleil
 - Translate Moon in your language   EX : Lune
 - Translate Season in your language   EX : Saison
 - Language  Suported lamguages da, de, en, es, fr, hu, it, nl, pl, ru, sl
 - Time format 12 hour, 24 hour

### Screenshots
**Light theme:**<br>


**Dark theme:**<br>


### Changelog
#### 1.0
- First release