# Prep for IoT PnP

Do this before the training

1. Flash SD Card with Raspbian Buster  
  2020-02-13-raspbian-buster-lite.zip
1. Add a empty file called `ssh` file to `boot` partition
1. Boot RP4 with the SD Card
1. Run :

```bash
ssh "pi@192.168.8.10" "cd ~/ && sudo apt-get update && sudo apt-get install -y git && git clone https://github.com/daisukeiot/IoT-Plug-and-Play-WS.git && cd IoT-Plug-and-Play-WS && /bin/bash ./prep-rp4.sh"
```

1. Flash SensorTile.Box firmware from <https://github.com/daisukeiot/IoT-Plug-and-Play-WS/blob/master/SensorTile.Box/IoT-PnP.bin>  
    Use STM32CubeProg to flash <https://www.st.com/en/development-tools/stm32cubeprog.html>
