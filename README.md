> [!WARNING]
> This project is **deprecated** and was superseded by [LoRaBridge2](https://github.com/lorabridge2). The replacement for **this** repository is [here](https://github.com/lorabridge2/gateway-ha_integration).

# Gateway Home Assistant Integration

This repository is part of the [LoRaBridge](https://github.com/lorabridge/lorabridge) project.
It provides the docker image for the Home Assistant integration software used on our gateway device.

The HA Integration is a self-provided Python3 application. 
It translates the MQTT messages sent by the Device Manager into messages understood by the MQTT integration of Home Assistant.

## Environment Variables

- `HA_MQTT_HOST`: IP or hostname of MQTT host
- `HA_MQTT_PORT`: Port used by MQTT
- `HA_MQTT_USERNAME`: MQTT username if used (can be a file as well)
- `HA_MQTT_PASSWORD`: MQTT password if used (can be a file as well)
- `HA_DISCOVERY_TOPIC`: MQTT topic used for announcing newly discovered devices (default: `lorabridge/discovery`)
- `HA_STATE_TOPIC`: MQTT topic used for announcing states (measurements) of devices (default: `lorabridge/state`)

## License

All the LoRaBridge software components and the documentation are licensed under GNU General Public License 3.0.

## Acknowledgements

The financial support from Internetstiftung/Netidee is gratefully acknowledged. The mission of Netidee is to support development of open-source tools for more accessible and versatile use of the Internet in Austria.
