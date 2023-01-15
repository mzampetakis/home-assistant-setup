# Application

Home Assistant can be installed in various OSs providing this way an integration with home/household devices. Such devices can be PCs, smartphones and laptops. This can be done through the [HA Companion App](https://companion.home-assistant.io/).

Using a HA client setup in a machine will allow us to exploit any sensor provided by these in order to integrate more things and generate even more complex automations and scenes.
There is an extensive list of sensors that HA companion app can access in a smartphone and provide them to the HA service. A list can be found at [this link](https://companion.home-assistant.io/docs/core/sensors).

A pretty common usage for this is to use the location sensor of a smart phone and apply different scenes when none is at home. A usage I have come app with is to turn on a light bulb to red whenever I am on a call within my home-office. This is pretty easy using the HA companion app in the MacOS which allows access to mic and camera status. This is the setup of the automation I am currently using:

```yaml
- id: '1665985594769'
  alias: When MZ camera turns on turn on to red light bulb 1
  description: ''
  trigger:
  - type: turned_on
    platform: device
    device_id: 7faacab9c31789f5cfe295cc1e536fe6
    entity_id: binary_sensor.macos_camera_in_use
    domain: binary_sensor
  action:
  - service: scene.turn_on
    target:
      entity_id: scene.turn_on_light_bulb_1_to_red
    metadata: {}
  mode: single
- id: '1665985797266'
  alias: 'When MZ camera turns off turn off light bulb 1 '
  description: ''
  trigger:
  - type: turned_off
    platform: device
    device_id: 7faacab9c31789f5cfe295cc1e536fe6
    entity_id: binary_sensor.macos_camera_in_use
    domain: binary_sensor
  action:
  - service: scene.turn_on
    target:
      entity_id: scene.turn_off_light_bulb_1
    metadata: {}
  mode: single
```

