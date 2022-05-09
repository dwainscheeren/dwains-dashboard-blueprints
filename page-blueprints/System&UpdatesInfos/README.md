# System And Update Info

This blueprint is partly an assembly of two Blueprints created by  [xBoumer](https://github.com/xBourner).

## Installation of this Blueprint
- Install mushroom-title-card from [HACS]
- Install mushroom-entity-card from [HACS]
- Install mushroom-update-card from [HACS]
- Install mini-graph-card from [HACS]
- Install bar-card from [HACS]
- Install auto-entities from [HACS]
- Install card-mod from [HACS]

- Install this Integration in Home Assistant. [Speedtest](https://www.home-assistant.io/integrations/speedtestdotnet/)

You need at least these arguments:

```
sensors:
- platform: systemmonitor
  resources:
    - type: disk_use_percent
      arg: / 
    - type: memory_use_percent      
    - type: processor_use     
    - type: processor_temperature
    - type: last_boot
    - type: ipv4_address
      arg: eth0
    - type: throughput_network_in
      arg: eth0
    - type: throughput_network_out
      arg: eth0
```      
- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to defines.
 - Translate speedtest in your language
 - Translate download in your language
 - Translate upload in your language 
 - Translate system in your language
 - Translate ip adress in your language
 - Translate Throughput out your language
 - Translate update in your language
 - Show or hide buttons controls  

### Screenshots
**Light theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/167270373-7228f9fa-f0ab-47b2-b349-38fd64ea9a38.jpeg)
![image](https://user-images.githubusercontent.com/83040228/167270376-3c7675b1-96e8-4ddb-b446-3d974ffac8bb.jpeg)

**Dark theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/167270391-529b93aa-9ee5-4975-9be3-108af963dca2.jpeg)
![image](https://user-images.githubusercontent.com/83040228/167270399-d4b3e17d-bb6c-4cab-a812-b8b3b3b26cd3.jpeg)

### Changelog
#### 1.0
- First release
