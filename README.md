# LoRa Network @ AoLab
## Introduction
In AoLab we have LoRa based networks with some gateways and ndoes.
In this repository we want to document information about this network and its assets.

## Gateways
Gateways connect the end devices to the [LoRa Gateway Bridge](https://www.loraserver.io/lora-gateway-bridge/overview/) with UDP port 1700.

```json
{
	"SX127x_conf":
	{
		"freq":          904100000,
		"spread_factor": 7,
		"pin_nss":       6,
		"pin_dio0":      7,
		"pin_rst":       0,
		"pin_led1":      4
	},
	"gateway_conf":
	{
		"ref_latitude":  0.0,
		"ref_longitude": 0.0,
		"ref_altitude":  10,
		"name":          "Single Channel Gateway",
	        "email":         "jaber.babaki94@gmail.com",
		"desc":          "Single Channel Gateway on RPI",
		"servers":
                [
			{
				"address": "172.23.132.37",
				"port":    1700,
				"enabled": true
			}
		]
	}
}
```
