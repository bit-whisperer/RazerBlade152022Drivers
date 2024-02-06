# Razer Blade 15 2022 Drivers
This is a repository for the extracted drivers from the Windows recovery image.

Right click on a device in device manager and click update driver to use these folders.

KEY:

DKM - Human Interface Devices -> USB Input Device

MOU - Mouse

KBD - Keyboard

The audio driver can be pulled from windows update, but if it still cannot be found, you can download the newest driver (7-12-22) realtek audio driver and place that in the driverstore with the software linked below. Or you can use the older OEM one from the recovery image. I placed both in there so you can try either one: https://mega.nz/folder/JKpg0CzR#Fpz_skNCHcIkMq6yx_AN-A

If you are experiencing audio dropouts like I was, you have to remove the THX spatial audio extension. I put instructions on how to do that in the "To Fix Audio" directory.

Use this to add the audio driver to the driverstore and delete the old one: https://github.com/lostindark/DriverStoreExplorer/releases

I was unable to find what the rest were for, but the three listed above were the ones I was successfully able to find and update.

# Trackpad Gestures Not Working after Sleep Fix

See this razer insider post: https://insider.razer.com/systems-14/touchpad-scrolling-not-smooth-razer-blade-17-2022-41416?postid=175194#post175194

I created this fix and I can confirm that it works. If Razer addresses this with a BIOS update I will update this readme.

# Trackpad jumpy tracking fix

Big thanks to Nukley for this fix. This fix is derrived from https://github.com/Nukley/SynapticsUnfuckerator2

Set the registry value Computer\HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\PrecisionTouchPad\AAPThreshold to 0. You will instantly feel the tracking be more responsive or less jumpy. If its still jumpy, clean the trackpad.


