---
icon: material/home
---

# :material-alert: Unreal Engine 5 Update makes this documentation irrelevant, please wait for a port of this in the future :material-alert:

# This is being actively updated, do not use this until finished

# :material-home: Welcome to the Payday 3 Wwise/Event Audio Modding Guide!

Now a little more Linux Friendly

Returning users from the original google doc, should go through the First Time Setup again. I promise this is the last time, and is required for proper following of the guides.

“What are the benefits of replacing audio with Events instead of just using [this](https://modworkshop.net/mod/51045) <span class="dark">:Icons-mws_logo_white:</span><span class="light">:Icons-mws_logo_black:</span>?”

Some of the more “simple” mods can use the PD3AudioModder tool, like replacing some small sound effects in the game. But some audio can have some strict expectations and can play weird/cut off with just simply replacing the audio directly without Wwise Events, or can even be impossible because of the way audio is handled in Papaya 3.

With Event replacing, the audio can be as long as you want and can be fancy with transitions, strict list of audio to play, sequences, control of which audio to play randomly, and potentially more! 

It will also have the advantage of making mods smaller in size with compression methods built into Wwise Unreal integration, and not needing to have the same audio file copied several times to replace multiple audio sounds.

## Tools to install

Repak - Even though modding no longer uses *just* .pak files, it's still requried to have one .pak file to contain the Wwise media (your audio files) for your events to play, [this tool](https://modworkshop.net/mod/50337) <span class="dark">:Icons-mws_logo_white:</span><span class="light">:Icons-mws_logo_black:</span> makes it slightly easier to make them.

File Converter - I use [this tool :fontawesome-brands-windows:](https://file-converter.io/?from=readme.md) to easily and locally convert files, instead of relying on online tools and their restrictions.

File Converter (Linux) - If you use Linux, you can use [this tool :simple-linux:](https://github.com/Lich-Corals/linux-file-converter-addon) to convert local files just as easy.

## Images

If you find some of the images hard to see, you can Right Click on them and "Open Image in New Tab" for a higher resolution view.

## Getting started

If you're starting out for the first time, navigate to either [:fontawesome-brands-windows: Windows](./First Time Setup/First Time Setup Windows/Windows.md) or [:simple-linux: Linux](./First Time Setup/First Time Setup Linux/Linux.md)

----

??? "Current Progress/Planned"
    - [x] First Time Setup

    - [ ] Tips

    - [ ] Wwise Information

    - [x] Audio Obstruction

    - [x] Standard Enemies SFX

    - [ ] Standard Enemies Voice Lines
        - [x] Guards & SWAT
        - [x] Police
        - [ ] Smalltalk Police
        - [x] Dispatch Pager Speech
        - [x] Radio Dispatcher
        - [x] First Responder Megaphone

    - [ ] Specials SFX
        - [x] Bulldozer
        - [x] Cloaker
        - [ ] Nader
        - [x] Shield
        - [ ] Sniper
        - [x] Techie
        - [x] Zapper

    - [ ] Specials Voice Lines
        - [x] Bulldozer
        - [x] Cloaker
        - [x] Nader
        - [x] Shield
        - [x] Techie
        - [ ] Drones
        - [x] Zapper

    - [x] FBI

    - [ ] Shade - Core Heists
    - [ ] Shade - Side Hustles
    - [ ] Shade - The Bad Apple
    - [ ] Shade - Smash & Grab
    - [ ] Shade - Tutorials

    - [ ] Subtitle integration

    - [ ] Building SFX
        - [x] Alarms
        - [x] Elevator
        - [ ] Night Club Music

    - [ ] Player Interactions
        - [x] Player Phone
        - [ ] Elevator Prying
        - [x] Radio Lure

    - [ ] Player Overkill Weapons
        - [x] Sociopath
        - [ ] Potentially more

    - [x] Mod Add-ons

    - [ ] Misc.
        - [x] Main Menu Music Event
        - [ ] Phone Hacking Circle
        - [x] Overkill Delivery Drone

    - [x] Paking Your Mod

    - [x] Paking Your Heist Jukebox Mod

    - [x] Paking Your Main Menu Jukebox Mod

??? "Current Versions"
    Wwise Project ver `0.8.5`

    Unreal Engine Project ver `1.0`

    Guide ver `0.8.5`
