# :sauropod: nanosaur-NX-shield - [![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]
🦸 A nanosaur NX, need a super shield. The Nanosaur NX shield is here!

NanoSaur is a little tracked robot ROS2 enabled, made for an NVIDIA Jetson Nano

If you need an extra support, below all links:
* :sauropod: Website: [nanosaur.ai](https://nanosaur.ai)
* :unicorn: Do you need an help? [Discord](https://discord.gg/NSrC52P5mw)
* :toolbox: For technical details follow [wiki](https://github.com/rnanosaur/nanosaur/wiki)
* :whale2: Nanosaur [Docker hub](https://hub.docker.com/u/nanosaur)
* :interrobang: Something wrong? Open an [issue](https://github.com/rnanosaur/nanosaur/issues)

# How make Nanosaur PCBs on PCBWay

- Register to PCBWay using [my refferer link](https://www.pcbway.com/setinvite.aspx?inviteid=472567)
- and ... **Work in progress!**

# Board design

This board is a simple adapter to connect the motor controller and the LCDs to the NVIDIA Jetson on your NanoSaur, this board connect:

* I2C bus 0 (Pin 27, 28)
  * oled right
* I2C bus 1 (Pin 3, 5)
  * oled left
  * adafruit motor control
* 2 custom buttons
  * GPIO Pin 31
  * GPIO Pin 33

## NVIDIA Jetson Reference

* Jetsonhacks [Jetson Nano pinout](https://www.jetsonhacks.com/nvidia-jetson-nano-j41-header-pinout/)

# Develop

The documentation is made using [Kicad](https://www.kicad.org/) 5

The CI is made using
* [Kibot](https://github.com/INTI-CMNB/KiBot)
* [kicad-exports](https://github.com/nerdyscout/kicad-exports)

# License

This project is under license [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
