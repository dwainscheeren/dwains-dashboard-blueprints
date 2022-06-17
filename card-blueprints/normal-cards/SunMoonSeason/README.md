# SunMoonSeason Blueprint

## Installation of this Blueprint

- Install compass-card from [HACS]
- Install sun-card from [HACS]

## Integrations

- This card needs the following three integrations to work.

## Sun

This integration is by default enabled, unless you’ve disabled or removed the default_config: line from your configuration. If that is the case, the   following example shows you how to enable this integration manually:

  ### Example configuration.yaml entry

    sun:

## Moon

To enable the moon sensor, add the following lines to your configuration.yaml or your sensors file:

  ### Example configuration.yaml entry

    sensor:
       - platform: moon
       
## Season

To enable the season sensor, add the following lines to your configuration.yaml or your sensors file:

  ### Example configuration.yaml entry

    sensor:
       - platform: season

 ## Sun 2 sensors, Install and configure the [Sun 2 card](https://github.com/pnbruckner/ha-sun2)

# Sun image for compass

- Copy the Sun.png image in /config/www/images/. Note: This image can be anything you want, but it must have the name Sun.png

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for each card.

 - Translate Sun in your language
 - Translate Moon in your language 
 - Translate Season in your language 
 - Language  Suported lamguages da, de, en, es, fr, hu, it, nl, pl, ru, sl
 - Time format 12 hour, 24 hour

### Screenshots
**Light theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/160249760-d912186d-2b47-4e0a-b08b-4b7c8162af5a.jpeg)

**Dark theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/160249771-b8d018fe-f37a-4ad9-b5db-3dbfd695b2b1.jpeg)

### Changelog
#### 1.0
- First release
