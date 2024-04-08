#### Fork from
<https://github.com/SmartHome-yourself/sonoff-tx-ultimate-for-esphome>

#### Use
```
substitutions:
  name: "ultimate-01"
  friendly_name: "__Sonoff Ultimate 01"

  relay_count: "3"

  toggle_relay_1_on_touch: "false"
  toggle_relay_2_on_touch: "false"
  toggle_relay_3_on_touch: "false"

packages:
  smarthomeyourself.tx_ultimate: github://xenofex7/sonoff-tx-ultimate-for-esphome/tx_ultimate.yaml@main

esphome:
  name: ${name}
  name_add_mac_suffix: false
  friendly_name: ${friendly_name}

api:
  encryption:
    key: xxx

wifi:
  ssid: !secret wifi_ssid
  password: !secret wifi_password
```
