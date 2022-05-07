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

![image](https://user-images.githubusercontent.com/83040228/167269455-f3830b7c-f521-437b-bc17-3ece13571599.png)

![image](https://user-images.githubusercontent.com/83040228/167269456-718e7176-f220-4461-9e2f-2292f0e78cff.png)

**Dark theme:**<br>

![image](https://user-images.githubusercontent.com/83040228/167269465-766add73-346e-4938-9690-298fcfb898c6.png)

![image](https://user-images.githubusercontent.com/83040228/167269467-fa0f4184-ce64-406e-92aa-13e5e161e853.png)

### Changelog
#### 1.0
- First release
