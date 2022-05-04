# Recently Added / Upcoming Media Card

## Requirements
- Install Upcoming Media Card from [Upcoming Media Card] (https://github.com/custom-cards/upcoming-media-card)
- Install Radarr Upcoming Media from [Radarr Upcoming Media] (https://github.com/custom-components/sensor.radarr_upcoming_media)
- Install Plex Recently Added from [Plex Recently Added] (https://github.com/custom-components/sensor.plex_recently_added)
- Install Sonarr Recently Added from [Sonarr Upcoming Media] (https://github.com/custom-components/sensor.sonarr_upcoming_media)

### Example entry

## Plex Recently Added Media Intergration
```
- platform: plex_recently_added
  token: plex token
  host: hostname / ip address
  port: 32400
```

## Radarr Upcoming Media Intergration
```
- platform: radarr_upcoming_media
  api_key: api key
  host: hostname / ip address
  days: 30
  ssl: false
  theaters: false
  max: 10
  urlbase: /radarr
```

## Sonarr Upcoming Media Intergration
```
- platform: sonarr_upcoming_media
  api_key: api key
  host: hostname / ip address
  days: 30
  ssl: false
  max: 10
  urlbase: /sonarr
```

##### Created by [dayshiers](https://github.com/dayshiers)

### Screenshots
**Example:**<br>
![Example](https://github.com/dayshiers/dwains-dashboard-blueprints/blob/main/card-blueprints/Recently%20Added,%20Upcoming%20Media/AddedMedia.PNG?raw=true "Example")

### Changelog
#### 1.0.0
- First release
#### 1.0.1
- Update Instructions
- Remove Horizontal Stack dependency
---
