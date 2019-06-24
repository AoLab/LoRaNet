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

Gateway is set up on the RPi device with the following information:

|             |                  |
| ----------- | ---------------- |
| mac address | b827ebffff70c80a |
| user        | pi               |
| pass        | jaber6600000     |


## End Devices
End devices connect to the gateway and send/recieve information through it.

Device address: `26 01 1b 84`

Network session key: `b6 66 ea 9c 9a ff 94 7c f3 37 79 77 55 f6 69 34`

Application session key: `c0 b2 c7 46 17 4d 82 f1 be 49 88 b8 08 63 63 f2`

LoraWan Mac version: `1.0.1`

Device EUI: `00a9fd1d3591f99f`
