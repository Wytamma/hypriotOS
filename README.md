# hypriotOS

<https://github.com/hypriot/flash>

`flash -u wifi-user-data.yml -bootconf no-uart-config.txt https://github.com/hypriot/image-builder-rpi/releases/download/v1.10.1/hypriotos-rpi-v1.10.1.img.zip`  

## Set up for temp sensor

sudo raspi-config  

<https://learn.adafruit.com/adafruits-raspberry-pi-lesson-11-ds18b20-temperature-sensing/ds18b20>

confim with `lsmod | grep -i w1_`

## Start

`docker-compose up -d`

You can copy the json from `flows_example.json` for a flow that tweets the temperature every 15 min. This requires a twitter dev account (i.e. API keys).
