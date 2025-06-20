# koleos_DPF_alert

**koleos_DPF_alert.bin** is a proprietary ESP32 binary application designed for Renault Koleos GEN1 (2007 - 2016) 2.0L dCi AWD variant. It reads DPF data and notifies the owner when a DPF regeneration begins and ends. This repository is for distribution purposes only.


# What does this app do?
1. It runs on a ESP32 that is mounted on a PCB. Lets call this PCB the 'dongle'. 
2. This dongle connects to your koleos OBD2 port and reads DPF relevant data and determines if a DPF regeneration event begins or ends. 
3. The dongle alerts the owner using a buzzer. 
    - Six(6) short beeps(0.1 seconds beep followed by 0.1 seconds pause) means a DPF regeneration started.
    - Three(3) long beeps (0.5 seconds beep followed by 0.5 seconds pause) means the DPF regeneration ended.


# Making the dongle:
- If you want to buy the dongle, send me an e-mail casianb3@gmail.com and maybe we can work something out.
- If you want to build your own dongle, I've provided the electrical schematic (look into the 'schematic' folder).

# Guide how to flash binary file to the ESP32: 
1. Follow this guide https://docs.espressif.com/projects/esp-test-tools/en/latest/esp32/production_stage/tools/flash_download_tool.html
2. Configure as in picture and press START: 
![ESP32 Flashing guide screenshot](assets/flashing-guide.png)


# Apps for the donle:
- Since the esp32 has bluetooth capabilities, I also developed some apps for the dongle. (TODO add more info, pictures, yt video links, etc)



## ⚠️ Licensing and Usage

This binary is **not open source**. Redistribution, modification, commercial use, or reverse engineering is **strictly prohibited** without prior written consent.

See [LICENSE](./LICENSE) for more details.

## 🔗 Third-Party Acknowledgments

This project integrates the [NimBLE-Arduino](https://github.com/h2zero/NimBLE-Arduino) library, licensed under the Apache License 2.0. See [NOTICE](./NOTICE) for attribution and license terms.

