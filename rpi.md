# Raspberry Pi first time setup

### Before turning it on

1.  Hook up the following components:

*   HDMI Cable
*   WiFi Dongle
*   Keyboard/Mouse
*   USB Drive (if you have one)

3.  Plug in the Power Cable
4.  Wait for bootup. You should see text scroll. It will boot directly to the desktop.
5.  That's it!

### Configuration

Click the internet Icon top right corner of the screen and connect to your local WiFi (At LLTC, that's Public.Wireless)

#### Click on Menu > Preferences > Raspberry Pi Configuration. Configure the following items:

1.  "System" Tab
    *   Click Expand Filesystem
    *   Click Change Password and change the password.
    *   Choose a hostname
    *   Add to Rastrack if you wish (It's just a fun website that shows where there are Pis active around the world.
2.  "Interfaces" Tab
    *   Camera: Disabled
    *   SSH: Enabled (I'll show you how to use this)
    *   SPI & I2C: Disabled (Pretty advanced stuff)
    *   Serial: Enabled (USB ports and such)
3.  "Performance" Tab
    *   Overclock: 1000MHz is pretty stable, but 900MHz is fine if you're nervous.
    *   GPU Memory: Pick a number between 256-512\. I usually use 512 when I intend to use the desktop.
4.  "Localization" Tab
    *   Locale: Language English, Country US, Character Set UTF-8 (The only thing you should have to change is the Country, which defaults to Great Britain)
    *   Timezone: US > Central
    *   Keyboard: United States > English(US)
5.  Hit "OK" and reboot.

### Software:

1.  Click on the Terminal icon on the top bar
2.  In the terminal type the following commands to update your packages and software to their newest bleeding edge versions:
    *   sudo apt-get update
    *   sudo apt-get upgrade
3.  Install a new Web Browser:
    *   sudo apt-get install iceweasel
4.  Install Git GUI - Git will be the primary way that we will submit programming assignments. It can be a little arcane, but I will explain how it all works as we go along.
    *   sudo apt-get install git-gui
