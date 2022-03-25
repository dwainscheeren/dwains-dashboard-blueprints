# ClockWeatherCalendar Blueprint

## Installation of this Blueprint

- digital-clock from [HACS]
- atomic-calendar-revive from [HACS]
- ha-card-weather-conditions from [HACS]

- This card needs the following two integrations to work.

##Sun

    This integration is by default enabled, unless you’ve disabled or removed the default_config: line from your configuration. If that is the case, the following example shows you how to enable this integration manually:

  # Example configuration.yaml entry

    sun:

##Moon

    To enable the moon sensor, add the following lines to your configuration.yaml or your sensors file:

  # Example configuration.yaml entry

    sensor:
       - platform: moon

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for each card.

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


**Dark theme:**<br>


### Changelog
#### 1.0
- First release