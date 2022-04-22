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

**Card**

![image](https://user-images.githubusercontent.com/83040228/164761936-cae5fdbf-eec4-447e-b7e9-8cb6519fc824.jpeg)

**Pop-Up**

![image](https://user-images.githubusercontent.com/83040228/164761983-c3a5b43b-f7b3-4896-a0e6-49cc7d65ba20.jpeg)

**Dark theme:**<br>

**Card**

![image](https://user-images.githubusercontent.com/83040228/164762044-a297c503-a574-47bc-bfc9-00336d8e25e4.jpeg)

**Pop-Up**

![image](https://user-images.githubusercontent.com/83040228/164762097-b923b91f-d5f4-4988-b057-bf2166956ab6.jpeg)

### Changelog
#### 1.0
- First release
