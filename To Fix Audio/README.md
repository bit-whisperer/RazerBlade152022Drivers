# How to fix audio dropouts on the Razer Blade 15 2022

To fix the audio dropouts, you have to uninstall the THX Spatial Audio.

First turn off automatic driver downloads through windows update. This can be done in Windows Settings App -> System -> About -> Advanced System Settings -> Hardware -> Device Installation Settings -> No -> Ok

There are other ways to disable it too, just do a serch for "disable automatic driver downloads from windows update windows 10"

Now the THX Spatial Audio can be removed without it being automatically reinstalled.

This can be done by using DriverStoreExplorer. https://github.com/lostindark/DriverStoreExplorer/releases

Delete any of the ones that say THX and then restart the computer.

Next install EqualizerAPO. I made an EQ preset to get you started. It's in this folder.

Apply it by overwriting the existing config in the EqualizerAPO\config directory and restart EqualizerAPO or your computer.

Enjoy sound that does not have a dynamic range compressor applied to it.
