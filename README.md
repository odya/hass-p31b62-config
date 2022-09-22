# hass-p31b62-config
Home Assistant & Node-Red configs for my long running P31B62 smart home project. That, unfortunately, was ended by russian invasion of Ukraine 🤬.


## Contents:
- [Main HASS config](configuration.yaml)
- Included HASS configs
  - `conf_*.yaml`
  - `automations.yaml`
  - `scripts.yaml`
  - `groups.yaml`
  - `scenes.yaml`
  - `customize.yaml`
  - `secrets.yaml` is not included. You need to create it by yourself
- [Node-Red flows](node-red/flows.json)
- [Xiaomi vacuum voice pack with maximized gain](www/leather_bastards_max.pkg)
- [ESPHome](http://esphome.io) device configs organized as separate repositories
  - [PetNet SmartFeeder](https://github.com/odya/hass-p31b62-config/wiki/PetNet-SmartFeeder-revival) `workroom_feeder.yaml` - Return your PetNet SmartFeeder (gen.1) back to life using external controller and integration to Home Assistant ecosystem. Requires soldering skills.
  - [Ajax Gateway](https://github.com/odya/hass-p31b62-config/wiki/Ajax-Gateway) `home_gateway_ajax.yaml` - Detects armed/disarmed status of [Ajax](https://ajax.systems) home security system using [Ajax Siren](https://ajax.systems/ua/products/homesiren/)
  - [Water heater temperature monitor](https://github.com/odya/hass-p31b62-config/wiki/Boiler-temperature-monitor) `bath_boiler_temp.yaml` - tracks temperature deltas using two sensors on water heater hot and cold pipes. Using deltas you can suppose that hot/cold valve is open or that hot water in a boiler is ending.
  - [Smart socket with power monitor and protections](esphome/bedroom_power_pc.yaml) `bedroom_power_pc.yaml` - Blitzwolf SHP-6 socket config. Provides power monitoring and ability to set overcurrent/overvoltage thresholds.
  - [Cheap module air quality monitor](esphome/home_air_monitor.yaml) `home_air_monitor.yaml` - Monitor your air quality using single platform and module replaceable components. Sensor list: PM, TVOC, eCO2, temperature, humidity, air pressure
  - [Ventilation control](esphome/kitchen_vent.yaml) `kitchen_vent.yaml` - Simple two-speed vent fan control.
  - [Outdoor climate sensor](esphome/outdoor_climate.yaml) `outdoor_climate.yaml` - Simple outdoor temperature/humidity sensor.
