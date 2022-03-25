# Recently Added / Upcoming Media Card

## Requirements
Install Upcoming Media Card from [HACS]
Install Radarr Upcoming Media from [HACS]
Install Sonarr Intergration from ![Sonarr](https://www.home-assistant.io/integrations/sonarr/ "Sonarr")

### Example sensors.yaml entry
## Radarr Intergration
- platform: radarr
  api_key: Api Key from Radarr
  host: Radarr Host Name / IP Address
  urlbase: /radarr
  monitored_conditions:
    - upcoming
    - diskspace
    - status
    - movies
  days: 10
  unit: TB

##### Created by [dayshiers](https://github.com/dayshiers)

### Screenshots
**Example:**<br>
![Example](https://github.com/dayshiers/dwains-dashboard-blueprints/blob/main/card-blueprints/Recently%20Added,%20Upcoming%20Media/AddedMedia.PNG?raw=true "Example")

### Changelog
#### 1.0.0
- First release

---
