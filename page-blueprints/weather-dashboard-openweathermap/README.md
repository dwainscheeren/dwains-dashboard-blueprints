<h1 align="center">Weather Dashboard - Dwains Dashboard Blueprint (more_page)</h1> 

Note: this blueprint is a ported addon from Dwains Dashboard Blueprints. This port is done by Robert Wilson. The original creator of this addon is Leon van der Linden.


<p align="center">Weather Dashboard in Home Assistant Dwains Dashboard.</p>


<p align="center">Created by <a href="https://github.com/rwilson131">Robert Wilson</a>
</p> 


<p align="center">
  <img src="https://user-images.githubusercontent.com/77990847/118019312-21797000-b359-11eb-8723-c4c2e49f4e7b.png" />
</p>




## Prerequisite
---
Make sure you have following installed this can be done manually or directly via hacs
- Cards
    - [state-switch](https://github.com/thomasloven/lovelace-state-switch)
    - [mini-graph-card](https://github.com/kalkih/mini-graph-card)
    - [auto-reload-card](https://github.com/ben8p/lovelace-auto-reload-card)
    - [Weather Card](https://github.com/bramkragten/weather-card)
    - [fontawesome icons](https://github.com/thomasloven/hass-fontawesome)
    - [Cupertino Icons](https://github.com/menahishayan/HomeAssistant-Cupertino-Icons)
    - [Button Card](https://github.com/custom-cards/button-card)
    - [HA card Weather Conditions](https://github.com/r-renato/ha-card-weather-conditions)
    - [fold-entity-row](https://github.com/thomasloven/lovelace-fold-entity-row)
    - [multiple-entity-row](https://github.com/benct/lovelace-multiple-entity-row)
    - [stack-in-card](https://github.com/custom-cards/stack-in-card)
    - [entity-attributes-card](https://github.com/custom-cards/entity-attributes-card)
- Integrations
    - OpenWeatherMap, untested with other weather integrations [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start?domain=openweathermap)
    
    - OpenUV [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=openuv)

    - IQVIA [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=openuv)

    - [nws_alerts](https://github.com/finity69x2/nws_alerts) hard coded for now
    
    - Sun [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=sun)

    - Moon [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=moon)

    - Seasons [![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=seasons)


<img width="618" alt="image" src="https://user-images.githubusercontent.com/77990847/114733529-b6ca1a00-9d43-11eb-876a-6f4beda466ec.png">



## Make Home Assistant integration 
---

### Determing Latitude and Longitude

- Choose `latitude` and `longtiude` from  [Google Maps](https://support.google.com/maps/answer/18539?hl=en&co=GENIE.Platform=Desktop) 

### IQVIA 
- Make the integration with [IQVIA](https://www.home-assistant.io/integrations/iqvia/)

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start?domain=iqvia)

### OpenUV
- To get the UV index card into the weather dashboard, make sure you have created a [API](https://www.openuv.io/) at [OpenUV](https://www.openuv.io/)
- After creating the API, install the [OpenUV](https://www.openuv.io/) integartion by clikking on the button below.
- [OpenUV](https://github.com/LRvdLinden/weather_dd_addon/blob/main/README.md#openuv)

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=openuv)

![image](https://user-images.githubusercontent.com/77990847/117784741-28fb2500-b244-11eb-945a-19dc8f3c3ab0.png)

## Sensors 
___
:warning: Please reboot Home Assistant after config the sensors! :warning:
### nws_alerts 
```yaml
- platform: nws_alerts
  zone_id: 'PAC049,WVC031'
```

## Installation of this Blueprint
---
- Copy the `blueprint.yaml` content into the Blueprint installation codeblock.


## Result
---
![image](https://user-images.githubusercontent.com/77990847/117791717-e426bc80-b24a-11eb-8bab-d0a70fbab8f3.png)

![image](https://user-images.githubusercontent.com/77990847/117780215-b720dc80-b23f-11eb-9158-36574841576c.png)

![image](https://user-images.githubusercontent.com/77990847/117789187-5ba71c80-b248-11eb-8ddc-45f8029a4936.png)

![image](https://user-images.githubusercontent.com/77990847/117780368-d91a5f00-b23f-11eb-88b8-741e067910aa.png)




---
Enjoy the work from Robert Wilson?

[![coffee](https://www.buymeacoffee.com/assets/img/custom_images/black_img.png)](https://www.buymeacoffee.com/rwilson131)
