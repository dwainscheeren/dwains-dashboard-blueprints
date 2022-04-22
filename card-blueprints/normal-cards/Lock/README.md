# Lock Blueprint

- This blueprint can be used as a card or as a pop-up.

## Installation of this Blueprint

- Install vertical-stack-in-card from [HACS]
- Install mushroom-lock-card from [HACS]

- Add the following sensor in the configuration.yaml or sensors.yaml file. The sensor is used to extract the states of the lock. Add your lock entity and translate the states into your language.

      - platform: template
        sensors:
          lock_translate_state:
          friendly_name: "Extract and translate lock status"
          value_template:  >
            {% if is_state('lock.xxxx_xxxx_xxx', 'locked') %} 
              Locked                           
            {% elif is_state('lock.xxxx_xxxx_xxx', 'locking') %} 
              Locking                                    
            {% elif is_state('lock.xxxx_xxxx_xxx', 'unlocked') %}
              Unlocked                      
            {% elif is_state('lock.xxxx_xxxx_xxx', 'unlocking') %}
              Unlocking                        
            {% else %}
              {{ states('lock.xxxx_xxxx_xxx') }} 
            {% endif %}         

- Restart Home Assistant

- Copy the content of the blueprint file `blueprint.yaml` into the Blueprint YAML code.

 ## Fields to define for each card.

 - Translate locked in your language
 - Translate unlocked in your language
 - The lock entity
 - Translate lock state in your language
 - Translate door state in your language
 - The door state entity
 - Translate operator in your language
 - The lock operator entity
 - Translate battery in your language
 - The lock battery entity

### Screenshots
**Light theme:**<br>


**Dark theme:**<br>


### Changelog
#### 1.0
- First release
