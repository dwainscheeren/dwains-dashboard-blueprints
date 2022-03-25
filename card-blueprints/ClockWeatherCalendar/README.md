# ClockWeatherCalendar Blueprint

## Installation of this Blueprint

- Install digital-clock from [HACS]
- Install atomic-calendar-revive from [HACS]
- Install ha-card-weather-conditions from [HACS]

 ## Integrations

- This card needs the following two integrations to work.

## Sun

 This integration is by default enabled, unless you’ve disabled or removed the default_config: line from your configuration. If that is the case, the   following example shows you how to enable this integration manually:

  ### Example configuration.yaml entry

    sun:


## Moon

To enable the moon sensor, add the following lines to your configuration.yaml or your sensors file:

  ### Example configuration.yaml entry

    sensor:
       - platform: moon



- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for this card.

 - Entity of the Calendar
 - Calendar no event text in your language Ex : Aucun événement pour aujourd'hui
 - Calendar no event text for next days in your language Ex : Aucun événement prochainement
 - Calendar full day event text for next days in your language Ex : Jour entier
 - Calendar until text in your language Ex : jusqu'au
 - Calendar maximun days to show
 - Weather card language en/it/nl/es/de/fr/sr-latn/pt/da/no-NO
 - temperatture Sensor
 - Condition Sensor (rain, sunny, cloudy, etc)  This is the state of the weather.xxxxxx entity
 - Feels like temperature Sensor
 - Humidity Sensor
 - Pressure Sensor
 - Visibility Sensor
 - Wind bearing Sensor
 - Wind peed Sensor


### Screenshots

**Light theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/160034776-61a66145-d304-4c21-95df-0f754535d891.jpeg)

**Dark theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/160034808-7ab3a112-4a32-4a58-8d86-c1af6ab240f0.jpeg)

### Changelog
#### 1.0
- First release
