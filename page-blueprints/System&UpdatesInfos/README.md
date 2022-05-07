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

- Install Speedtest Integration in Home Assistant. 
- Enable systemmonitor in your configuration.yaml.

You need at least these arguments:

```
sensor:
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
    - type: network_in
      arg: eth0     
    - type: network_out
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

**Dark theme:**<br>

### Changelog
#### 1.0
- First release
