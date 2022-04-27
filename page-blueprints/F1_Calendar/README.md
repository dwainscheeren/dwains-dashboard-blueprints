# F1 Calendar Blueprint

This Blueprint is a Blueprint version of F1_calendar page created by [Wolk9](https://github.com/dwainscheeren/dwains-dashboard-addons/tree/for-dd-2.0/more_page/f1_calendar).

### Prerequisite
- Make sure you have the [Google Calendar](https://www.home-assistant.io/integrations/calendar.google/) integration

### Installation

- Install button-card from [HACS]

- Add the [F1 2022 Calendar by Racefans](https://www.racefans.net/contact/f1-fanatic-calendar/) to your Google Calendar
- Restart home-assistant and open `google_calendars.yaml`, this file should be in the root folder (this is also where your configuration.yaml and secrets.yaml should be located)
- Find the calendar with device id `formula_1_calendar_by_racefans_net`, it should look like this;
```yaml
- cal_id: ekqk1nbdusr1baon1ic42oeeik@group.calendar.google.com
  entities:
  - device_id: formula_1_calendar_by_racefans_net
    ignore_availability: true
    name: Formula 1 calendar by RaceFans.net
    track: true
``` 
Replace it with the following;
```yaml
- cal_id: ekqk1nbdusr1baon1ic42oeeik@group.calendar.google.com
  entities:
  - device_id: formula_1_calendar_fp1
    ignore_availability: true
    name: Formula 1 - FP1
    track: true
    search: "FP1:"
  - device_id: formula_1_calendar_fp2
    ignore_availability: true
    name: Formula 1 - FP2
    track: true
    search: "FP2:"
  - device_id: formula_1_calendar_fp3
    ignore_availability: true
    name: Formula 1 - FP3
    track: true
    search: "FP3:"
  - device_id: formula_1_calendar_qualifying
    ignore_availability: true
    name: Formula 1 - Qualifying
    track: true
    search: "Qualifying:"
  - device_id: formula_1_calendar_race
    ignore_availability: true
    name: Formula 1 - Race
    track: true
    search: "Race:"
```
- Make sure the sensor configuration in `formula1.yaml` is loaded, either by copying it in the folder with your other sensors, or by copying and pasting the contents in your `sensors:` configuration (or any other way you have setup your custom sensors).
- Restart home assistant again, you will now find a formula 1 sensor in your entities overview.

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define.
 - Translate Location in your language
 - Translate Circuit in your language
 - Translate Free practice 1 in your language
 - Translate Free practice 2 in your language
 - Translate Free practice 3 in your language
 - Translate Qualifying in your language
 - Translate Race in your language

You can translate the dates as well, instead of using the English `formula1.yaml` sensor file, use the Dutch `formula1-translated.yaml` and change the second parameter in the `replace()` filters on lines 17, 21, 25, 29 and 33.

### Screenshots
**Light theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/165640441-eab40711-c78f-4868-a630-dc6cd6f113d6.png)

**Dark theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/165640456-73fa68d0-e5f7-4897-acd2-6e685e1bac44.png)

### Changelog
#### 1.0
- First release
