# CXG-E60WT Soldering Iron firmware (STM8S103K3)
# WORK IN PROGRESS

A firmware for new soldering irons with STM8S103K3 MCU onboard. Some missing features have been implemented, such es. sleep/wake up modes, sounds, errors check, etc. 

Just download main.hex file to load it directly with stm8flash or STVP-STM8 STM Visual Programmer.

For those who wants to re-build the firmware: you'll need two essential pieces of software to work with the STM8:

- stm8flash, a utility for interfacing your ST-Link dongle
* Package: [aur/stm8flash-git](https://aur.archlinux.org/packages/stm8flash-git/)
* GitHub: [vdudouyt/stm8flash](https://github.com/vdudouyt/stm8flash)
- SDCC, a compiler
* Package: [community/sdcc](https://www.archlinux.org/packages/?q=sdcc)
* [Home page](https://sourceforge.net/projects/sdcc/files/snapshot_builds/)

## On Linux:

### To install SDCC
```
sudo add-apt-repository ppa:laczik/ppa
sudo apt-get update
sudo apt-get remove sdcc sdcc-libraries
sudo apt-get install sdcc
```
### To install stm8flash
```
git clone https://github.com/vdudouyt/stm8flash.git
cd stm8flash
make
sudo make install
```

## CXG-E60WT Scheme

![CXG-E60WT Scheme](/images/scheme.gif)

## Additional hardware

The following additional hardware has been installed:
- Mercury Switch: https://www.aliexpress.com/item/32509962658.html?spm=a2g0s.9042311.0.0.274233edX3SZw4
- SMD Buzzer:   https://www.aliexpress.com/item/4000043864737.html?spm=a2g0s.9042311.0.0.274233ediyCCli


Please feel free to use, modify, add cool new features.  Bye!
