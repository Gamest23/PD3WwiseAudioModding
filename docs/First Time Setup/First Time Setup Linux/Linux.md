---
icon: simple/linux
---

# Linux

## Disclaimer

Unfortunately, there is no way to make Wwise Event mods "natively" on linux. Even with Wine or its forks like Proton.

This is due to [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/), as far as I'm concerned this cannot be "installed" within a Wine environment and have Unreal Engine/Wwise Launcher recognize it.

Currently the "best" way is to install a virtual machine software and set up Windows. 

!!! warning
    Unreal Engine **requires** DirectX support, so not all Virtual Machine software, like [VirtualBox](https://www.virtualbox.org/), can be used.

[VMware](https://www.vmware.com/) currently is the only program that has support for a "Virtual GPU". Maybe at somepoint the program [WinBoat](https://winboat.app/) can be used instead, when it does get proper Hardware Acceleration support. (last update 9/9/2026)

I am aware of some Virtual Machine software supports GPU Passthrough, though I am not familiar with it and thus will not be covered.

## Hardware Requirements

Running another operating system is not a light task, especially for the purpose of our use case.

[Officially](https://techdocs.broadcom.com/us/en/vmware-cis/vsphere/vsphere/7-0/esx-upgrade/upgrading-esxi-hosts-upgrade/esxi-requirements-upgrade/esxi-hardware-requirements-upgrade.html), the hardware requirements are as follows:

- 2 CPU cores

- 8GB of *physical* memory/RAM

- 32gb of free storage

**Though** in reality you are going to need:

- 6 CPU cores from 2017 (8th gen Intel or 3000 series of Ryzen AMD)

- 16gb of *physical* memory/RAM

- 256gb of free storage

If you are unsure what you have, look up your distro and how you can find your hardware specifications, it's not always universal.

If you don't meet these requirements, I don't recommend you try and run a virtual machine.

## Installing VMware

Installing VMware depends on what linux distro you use.

### :material-arch: Arch

sudo pacman -S vmware-workstation

or

sudo yay -S vmware-workstation

### :simple-linux: Other Distros

Other distros, like Ubuntu or Fedora, need specific instructions on installing VMware. I do not personally use said distros. My setup uses CachyOS, an Arch based distro.

These resources may be helpful if you do have either installed:

:material-ubuntu: [Installing VMWare Workstation Pro on Ubuntu Desktop](https://paulyu.dev/article/installing-vmware-on-ubuntu-desktop/)

:material-fedora: [How to actually install VMware Workstation on Fedora](https://gist.github.com/burritosoftware/b0d66e15cd9573b577cafda049e3c6a6)

----

[VMware Setup](../First%20Time%20Setup%20Linux/VMware%20Setup.md)