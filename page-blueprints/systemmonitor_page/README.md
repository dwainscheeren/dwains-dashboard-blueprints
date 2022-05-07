## Pi-Hole Blueprint Home-Assistant
## More_page for Dwains Dashboard v3
##### Created by Bourner
##### Note: This page is based on the work of [noodlemctwoodle](https://github.com/noodlemctwoodle). 
---

### HACS components

- Install [Mushroom Cards](https://github.com/piitaya/lovelace-mushroom) from [HACS](https://hacs.xyz).
- Install [Mini Graph Card](https://github.com/kalkih/mini-graph-card) from [HACS](https://hacs.xyz).
- Install [Bar Card](https://github.com/custom-cards/bar-card) from [HACS](https://hacs.xyz).
- Install [Fold Enitity Row](https://github.com/thomasloven/lovelace-fold-entity-row) from [HACS](https://hacs.xyz). 
- Install [Stack in Card](https://github.com/custom-cards/stack-in-card) from [HACS](https://hacs.xyz). 

### Configuration

Install Speedtest Integration in Home Assistant. 
Enable systemmonitor in your configuration.yaml.

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



### Installation: 
  
1.  Go to More Page on DD3
2.  Create a new more page
3.  Use Dwains Dashboard Blueprint
4.  Add YAML Code from file to HA
5.  Click install Blueprint
6.  Click Use this Blueprint


### Links:
* https://github.com/dwainscheeren/dwains-dashboard-blueprints
* https://www.home-assistant.io/

---

This is a Blueprint for System Monitoring + Speedtest + System Controls.
This will automatically show your system and speedtest in a dd3 page.

### Screenshots:

![image](https://user-images.githubusercontent.com/64064679/167079943-fa9571ef-1180-4c49-a8ab-ad4caa2f5a89.png)

### Changelog
#### 1.0.0
- First release
#### 2.0.0
- Added Shortcuts & Systemcontrols for 2022.5



