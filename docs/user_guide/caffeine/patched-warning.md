# Patched Switch Safety

There are many homebrew apps that were developed exclusively for RCM-vulnerable Switches. They do risky things under the assumption that people have their eMMC backed up, allowing the backup to be restored if the system is bricked.

Patched Switches cannot do this, requiring users to take extra cautions when running any homebrew. For this reason, it is important to only ever run homebrew inside an emuMMC, so Hekate can always run before booting into a modified NAND.

Additionally, there are several homebrew applications, such as AutoRCM enablers, that make changes to the Switch, even in emuMMC, and therefore should never be used.

The final thing to note is that the Switch keeps track of when it finds out an update is available. If your Switch ever connects to the internet without a safety DNS configured, it will discover that it is outdated, and refuse to boot the web browser. This is known as supernag, and cannot be removed on a patched Switch. It is still advised to not update over the internet, as there may be a way to remove supernag in the future.

#### [Continue to SD Preparation <i class="fa fa-arrow-circle-right fa-lg"></i>](sd_preparation.md)
