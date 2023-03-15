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

# Other Tweaks

You can add inertia scrolling on the trackpad back with a registry tweak.

HKEY_CURRENT_USER/Software/Microsoft/Wisp/Touch

In this directory, change "Friction" to 15 and log out and log back in.

If it doesn't apply the first time, restart until it does. It took me two restarts to get it applied the first time.

If it still doesn't apply, search for the Friction key and replace any ones that get found with 15.

After that, it will be persistent after every startup.

It may not work perfectly on 2% of programs, but at least it restores the functionality.

If palm rejection is not working correctly on the trackpad, you can increase the aggressiveness of the palm rejection.

HKEY_CURRENT_USER/Software/Microsoft/Windows/CurrentVersion/PrecisionTouchPad

Look for the AAPThreshold key and then set the value from 2 to 3. 0 will disable palm rejection.

