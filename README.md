# Home.app Style templates for HomeAssistant

![Lovelace](https://raw.githubusercontent.com/asierralozano/homeapp-templates/master/resources/HALovelace.PNG "Lovelace")

The main goal of this repo is to provide a wide range of differents templates that fit the "Home.app" style provided by Apple. 
We are right now supporting the following entities domains:
* alarms
* binary_sensors
* lights
* media_players (sound & video)
* switches
* weather

Of course, this is not a 1to1 match to the "Home.app" style. We have took the idea, and implemented it in our way.

**Keep in mind that this config ONLY WORKS on YAML mode**

# How to install it on HomeAssistant.
* First of all, you need to install HACS, because we need some cards from there.
* Once you have HACS installed, you need to install the following cards:
  * [button-card](https://github.com/custom-cards/button-card)
  * [decluttering-card](https://github.com/custom-cards/decluttering-card)
  * [light-entity-card](https://github.com/ljmerza/light-entity-card)
  * [browser_mod](https://github.com/thomasloven/hass-browser_mod)
  * [light-popup-card](https://github.com/DBuit/light-popup-card)
  * [switch-popup-card](https://github.com/DBuit/switch-popup-card)
* Clone this repo into the `config` folder on your HA installation
* Define the following lines on your lovelace `.yaml` file in which you are setting up your Lovelace UI (in my case, `ui-lovelace.yaml`):
```yaml
button_card_templates: !include_dir_merge_named homeapp-templates/templates/button-card
decluttering_templates: !include_dir_merge_named homeapp-templates/templates/decluttering-card
```

# TODOs
* Implement more entities domains
* Support themes
* Support variations of the existings cards
* Order a little bit some messy parts of the code

# Contribute
I would love to build a wide stardard templates that follows the "Home.app" style, so please! feel free to contribute!  
To do it, you just need to clone this repo, create a PR, and that's it!  
It would be awesome!

# Thanks!
I would also say thanks to every contributor and the authors of the resources that I'm using! Thanks guys! 