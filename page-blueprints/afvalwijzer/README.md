# Afvalwijzer Blueprint

Note: this blueprint is a ported addon from Dwains Dashboard v2 addons. This port is done by Dwain Scheeren. The original creator of this addon is Jeroen Klompen.

##### Created by [Jeroen Klompen](https://github.com/klumpke/)


### Installation of this Blueprint
- Install [auto-entities](https://github.com/thomasloven/lovelace-auto-entities) and [Afvalbeheer](https://github.com/pippyn/Home-Assistant-Sensor-Afvalbeheer) from [HACS](https://hacs.xyz).
- In the HomeAssistant GUI, go to `Configuration` -> `Lovelace Dashboards` -> `Resources` -> `+` and add the following information.
  - URL: /hacsfiles/lovelace-auto-entities/auto-entities.js
  - Resource type: JavaScript Module
- Download the [images ZIP file](https://github.com/Klumpke/dwains-dashboard-addons/blob/master/more_page/afvalwijzer/.github/afvalwijzer-images.zip) and extract it into your `<config dir>/www/images`  directory.
- Restart Home Assistant.
- Copy the content of the blueprint file `blueprint.yaml` into the blueprint installation block.


### Screenshots
**Light theme:**<br>
![light](https://github.com/Klumpke/dwains-dashboard-addons/blob/master/more_page/afvalwijzer/.github/screenshots/light.png "Light")

**Dark theme:**<br>
![dark](https://github.com/Klumpke/dwains-dashboard-addons/blob/master/more_page/afvalwijzer/.github/screenshots/dark.png "Dark")


### Changelog
#### 1.0.0
- First release

---

If you like the work of Jeroen Klompen:

<a href="https://www.buymeacoffee.com/klumpke" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/white_img.png" alt="Buy Me A Coffee"></a>
