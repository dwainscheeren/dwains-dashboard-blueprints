## Docker Monitor Blueprint Home-Assistant
## More_page for Dwains Dashboard v3
##### Created by Bourner
---

### HACS components

- Install [simpleicons](https://github.com/vigonotion/hass-simpleicons) from [HACS](https://hacs.xyz).
- Install [Monitor-Docker](https://github.com/ualex73/monitor_docker) from [HACS](https://hacs.xyz).

### Configuration

You can select all conditions and containers but at least you need these as minimum config.
You can also rename your containers to have you own name otherwise the default docker name is chosen. 

```
- monitor_docker:
  - name: Docker
    url: tcp://127.0.0.1:2375
    rename:
      portainer: Portainer
      npm_app_1: 'Nginx Proxy App'
    monitored_conditions:
      - containers_running
      - containers_total
      - containers_paused
      - containers_stopped
      - state
      - status
      - memory
      - cpu_percentage
      - uptime
      - network_total_up
      - network_total_down
      - network_speed_up
      - network_speed_down 
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

This is a Blueprint for Docker Monitor.
This will automatically pull all your docker containers and show them in a dd3 page.

### Screenshots:

![image](https://user-images.githubusercontent.com/64064679/162574406-7ea6481a-e592-4a03-bc9b-c368b35bd880.png)

![image](https://user-images.githubusercontent.com/64064679/162574447-334c4835-6d41-413b-8313-7952ed15009b.png)

### Changelog
#### 1.0.0
- First release
#### 2.0.0
- Changed working behaviour to auto-entities-card
#### 2.1.0
- Added units
