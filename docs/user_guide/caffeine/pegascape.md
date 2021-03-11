# Using PegaScape

PegaScape is a webpage that contains useful exploits for the Switch. On firmwares 2.0.0-4.1.0, there are two free ways to access the browser that PegaScape supports.

The first entrypoint is the WiFi registration prompt. Starting on 2.0.0, joining a WiFi network that requires a login page will load the internet browser to complete the registration, allowing public WiFi networks to be joined. However, the Switch uses a domain name for this, meaning it can be redirected to PegaScape using DNS.

The other entrypoint is within the News Applet. While most news entries use HTTPS, Fake News Injector can be used to add an HTTP entry. However, Fake News Injector also requires one-time access to homebrew beforehand, which is usually PegaScape through the WiFi prompt.

----

### Launching PegaScape from the Internet Browser
1. Delete any existing WiFi configuration that you are connected to.
2. Connect to a password-protected WiFi network, but instead of typing the correct password, spam the keyboard.
3. The connection test should fail. Open the network configuration.
4. Set the DNS configuration to manual.
5. Set the primary DNS to `51.15.245.41`
6. Set the secondary DNS to `163.172.141.219`
7. Enter the correct password. You should be told that that WiFi network requires login.
8. PegaScape should now load.

!!! tip ""
- If you are told to update before using the browser, your console is under supernag.
- Do not update the console. This will block your access to PegaScape.
- If your Switch is patched, you cannot access homebrew at this time. It is still advised not to update, however, because there might be a way to remove supernag in the future.
- If your Switch is not patched, use [RCM](../rcm.md) to launch CFW. Afterward, place <a href="https://github.com/Adubbz/Gag-Order/releases" target="_blank">Gag-Order</a> in SD:/switch and launch it from hbmenu.

----

### Injecting Fake News
Make sure PegaScape is open before continuing.
1. Press hbmenu.
2. Press HOME to exit the browser.
3. Open the Album. hbmenu should load instead of the Album.
4. Launch Fake News Injector.
5. Press + to install fake news.
6. Press + to reboot.
7. When the Switch boots, return to network settings.
8. Set the primary DNS to `163.172.181.170`
9. Save the settings. The connection test should succeed.

----

### Rebooting to Hekate
This is the only part that must be repeated on every boot.
1. Open News.
2. Load the "Launch PegaSwitch" news entry. (while PegaSwitch is a different app, PegaScape uses similar components, so this news entry can also launch PegaScape)
3. When PegaScape loads, press the coffee icon to load Caffeine.
4. Tap the textbox that appears. No keyboard should load.
5. After 3-5 seconds, press (don't hold) the power button to sleep.
6. Press the power button again to wake up from sleep. Hekate should load.

#### [Continue to partitioning the SD card (emuMMC CFW) <i class="fa fa-arrow-circle-right fa-lg"></i>](../emummc/partitioning_sd.md)

#### [Continue to Making Essential Backups (sysNAND CFW) (**Not Recommended, especially for patched Switches**) <i class="fa fa-arrow-circle-right fa-lg"></i>](../sysnand/making_essential_backups.md)
