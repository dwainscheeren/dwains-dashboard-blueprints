## Docker Monitor Blueprint Home-Assistant
## More_page for Dwains Dashboard v3
##### Created by Holewijn
---

### HACS components

- Install [button-card](https://github.com/custom-cards/button-card) from [HACS](https://hacs.xyz).
- Install [bar-card](https://github.com/custom-cards/bar-card) from [HACS](https://hacs.xyz).
- Install [mini-graph-card](https://github.com/kalkih/mini-graph-card) from [HACS](https://hacs.xyz).
- Install [swipe-card](https://github.com/bramkragten/swipe-card) from [HACS](https://hacs.xyz).
- Install [card-mod](https://github.com/thomasloven/lovelace-card-mod) from [HACS](https://hacs.xyz).

### Configuration

- Install [Mosquitto addon](https://github.com/home-assistant/addons/tree/master/mosquitto)  in HA, 
- Install [Unraid-API](https://hub.docker.com/r/electricbrainuk/unraidapi) from [Docker Apps](https://hub.docker.com/)
- Install [Glances](https://hub.docker.com/r/nicolargo/glances/) from [Docker Apps](https://hub.docker.com/) After install edit the docker container and and this to your repository nicolargo/glances:3.2.4.2-full latest version doesn't seem to work. 

### Installation: 
  
1.  Go to More Page on DD3
2.  Create a new more page
3.  Use Dwains Dashboard Blueprint
4.  Add YAML Code from file to HA
5.  Click install Blueprint
6.  Edit the blueprint to your liking if you have a other name of sensor or less/more harddisk's
7.  Click Use this Blueprint 

### Links:
* https://github.com/dwainscheeren/dwains-dashboard-blueprints
* https://www.home-assistant.io/

---

### Screenshots:
### Desktop
![image](https://user-images.githubusercontent.com/16470505/167884137-20774dce-68ae-4971-832d-4d3f17977c47.png)
### Mobile
![280323994_1075084656553174_7319764932848544471_n](https://user-images.githubusercontent.com/16470505/167884949-62a9bc71-471e-482d-8cea-f0cec9bdc7b6.jpg)

This is a Blueprint for Unraid Monitoring.
This will automatically pull all your docker's, harddisk's & ssd and more stats and show them in a dd3 page.

### Changelog
#### 1.0.0
- First release
#### 1.1.0
- Added right side view
- Added Disk Array Temperature
- Dockers arranged from left to right. 
