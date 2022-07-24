# :sauropod: 🦸 nanosaur-NX-shield - [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[![Discord](https://img.shields.io/discord/797461428646707211)](https://discord.gg/YvxjxEFPkb) [![GitHub Org's stars](https://img.shields.io/github/stars/rnanosaur?style=social)](https://github.com/rnanosaur) [![Twitter Follow](https://img.shields.io/twitter/follow/raffaello86?style=social)](https://twitter.com/raffaello86) [![robo.panther](https://img.shields.io/badge/Follow:-robo.panther-E4405F?style=social&logo=instagram)](https://www.instagram.com/robo.panther/)

**nanosaur** The smallest [NVIDIA Jetson](https://developer.nvidia.com/buy-jetson) dinosaur robot, **open-source**, fully **3D printable**, based on [**ROS2**](https://www.ros.org/) & [**Isaac ROS**](https://developer.nvidia.com/isaac-ros-gems).

<small>Designed & made by [Raffaello Bonghi](https://rnext.it)</small>

[![nanosaur](https://nanosaur.ai/assets/images/banner.jpg)](https://nanosaur.ai)

Meet nanosaur:
* 🦕 Website: [nanosaur.ai](https://nanosaur.ai)
* 🦄 Do you need an help? [Discord](https://discord.gg/YvxjxEFPkb)
* 🧰 For technical details follow [wiki](https://github.com/rnanosaur/nanosaur/wiki)
* 🐳 nanosaur [Docker hub](https://hub.docker.com/u/nanosaur)
* ⁉️ Something wrong? Open an [issue](https://github.com/rnanosaur/nanosaur/issues)

# How make Nanosaur PCBs on PCBWay

- Register to PCBWay using [my refferer link](https://www.pcbway.com/setinvite.aspx?inviteid=472567)
- and ... **Work in progress!**

# Board design

This board is a simple adapter to connect the motor controller and the LCDs to the NVIDIA Jetson on your NanoSaur, this board connect:

* I2C bus 0 (Pin 27, 28)
  * oled right
  * IMU
* I2C bus 1 (Pin 3, 5)
  * oled left
  * adafruit motor control
  * USB [STUSB4500QTR](https://www.st.com/resource/en/datasheet/stusb4500.pdf)
* 2 custom LEDS
  * GPIO Pin 31
  * GPIO Pin 33

## NVIDIA Jetson Reference

* Jetsonhacks [Jetson Xavier NX pinout](https://www.jetsonhacks.com/nvidia-jetson-xavier-nx-gpio-header-pinout/)
* Jetsonhacks [Jetson Nano pinout](https://www.jetsonhacks.com/nvidia-jetson-nano-j41-header-pinout/)

## STUSB4500QTR

* [STUSB4500QTR](https://www.st.com/en/interfaces-and-transceivers/stusb4500.html)
* [Evaluation board EVAL-SCS001V1](https://www.st.com/content/st_com/en/products/evaluation-tools/solution-evaluation-tools/psu-and-converter-solution-eval-boards/eval-scs001v1.html)
* [ST Easy migration](https://www.st.com/resource/en/user_manual/um2586-fast-and-easy-migration-from-dc-barrel-to-typec-stmicroelectronics.pdf)
* [Github STUSB4500](https://github.com/usb-c/STUSB4500)
* [Sparkgun tutorial](https://learn.sparkfun.com/tutorials/power-delivery-board---usb-c-qwiic-hookup-guide)
* [Hackaday tutorial](https://hackaday.com/2019/10/18/usb-power-delivery-for-all-the-things/)
* [STM presentation](https://www.stmicroelectronics.com.cn/content/dam/AME/2019/technology-tour-2019/chicago/presentations/T1S3_Schaumburg_USB-Type-C_G.Gosciniak.pdf)

# Develop

The documentation is made using [Kicad](https://www.kicad.org/) 6

The CI is made using
* [Kibot](https://github.com/INTI-CMNB/KiBot)
* [kicad-exports](https://github.com/nerdyscout/kicad-exports)

# License

This project is under license [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
