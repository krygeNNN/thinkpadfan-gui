# Thinkpad Fan Tweaker GUI

<p align="left">
  <a href="https://github.com/krygeNNN/thinkpadfan-gui">
    <img src="Images/fan-icon-vector-15.png" alt="Logo" width="80" height="80">
  </a>
<p align="center">
  <a href="https://github.com/krygeNNN/thinkpadfan-gui">
    <img src="Images/thinkpadgui.png" alt="Logo" >
  </a>

## Description

Spesifically designed for ThinkPad and IBM laptops to tweak fan speed with a graphical user interface.
You can also monitor CPU, GPU temperatures.

### Dependencies

* Python3 libraries --> subprocess, shlex
* Unix binaries --> lm-sensors
* OS --> Any Linux kernel with `thinkpad-acpi` patch. 

### Installing
 ```
  git clone https://github.com/krygeNNN/thinkpadfan-gui.git
  pip3 install -r requirements.txt
  ```
Arch Based
  ```
  sudo pacman -S lm-sensors dmidecode
  ```
Debian Based
  ```
  sudo apt-get install lm-sensors dmidecode
  ```

### Setup

* `echo options thinkpad_acpi fan_control=1 | sudo tee /etc/modprobe.d/thinkpad_acpi.conf`
* Reboot your computer.
* Run script with `sudo`
```
sudo python3 thinkpad_fan_gui.py
```
