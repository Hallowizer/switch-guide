# Using PegaScape

PegaScape is a webpage that contains useful exploits for the Switch. On firmware 1.0.0, there are two Internet Browser entrypoints that can be used for PegaScape.

The first entrypoint is inside SEGA's Puyo Puyo Tetris. The digital manual for this game contains a link to SEGA's website, which opens on the Switch.

The other entrypoint is within the News Applet. While most news entries use HTTPS, Fake News Injector can be used to add an HTTP entry. However, Fake News Injector also requires one-time access to another entrypoint.

For this one-time entrypoint, either RCM or Puyo Puyo Tetris can be used.

----

### Configuring DNS
Regardless of how Fake News is injected, PegaScape's DNS server must be set.
1. If you are currently connected to a network, delete that network's configuration immediately.
2. Join a password-protected network, but spam the keyboard instead of typing the correct password.
3. When the authentication fails, change the settings.
4. Set the DNS configuration to manual.
5. Set the primary DNS to `163.172.181.170`
6. Set the secondary DNS to `163.172.141.219`
7. Enter the correct password to the WiFi network. The connection test should succeed.

----

### Using RCM
All Switches on firmware 1.0 should have access to RCM.

1. Enter RCM and inject Hekate.
#### [Continue to Entering RCM<i class="fa fa-arrow-circle-right fa-lg></i>"](entering_rcm.md)
2. Select "Launch"
3. Select sysMMC CFW.
4. Open the Album.
5. Launch Fake News Injector.
6. Reboot once finished.

----

### Using JP Puyo Puyo Tetris
If you do not already have Puyo Puyo Tetris installed, you will need a cartridge for it. DO NOT connect for the internet to access the eShop!
1. Launch JP Puyo Puyo Tetris.
2. Press A, then R, then A.
3. Press the bottom menu item.
4. Press SEGA at the bottom left. PegaScape should now load.

!!! tip ""
- If you are told to update before using the browser, your console is under supernag.
- Do not update the console. Firmware 1.0.0 contains many useful glitches that are not found in later firmwares, and the Switch contains anti-downgrade measures.
- To inject a news entry, follow the RCM method above.
- Afterward, when Hekate automatically loads, place <a href="https://github.com/Adubbz/Gag-Order/releases" target="_blank">Gag-Order</a> in SD:/switch and launch it by booting to CFW again.

5. Select Fake News Injector.

----

### Rebooting to Hekate
This is the only part that must be done every boot.
1. Load the News applet.
2. Select the news entry titled "Launch PegaSwitch" (note: while PegaSwitch is a different app, this news entry can also load PegaScape if the Switch is on PegaScape DNS)
3. Tap the video or the link.
4. Select Nereba on the PegaScape page.

#### [Continue to partitioning the SD card (emuMMC CFW) <i class="fa fa-arrow-circle-right fa-lg"></i>](../emummc/partitioning_sd.md)

#### [Continue to SD preparations (sysNAND CFW) (**Not Recommended**) <i class="fa fa-arrow-circle-right fa-lg"></i>](../sysnand/sd_preparation.md)
