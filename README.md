This is my modifications to the eggbot inkscape extension https://github.com/evil-mad/eggbot/releases EggBot_extensions_v281.zip to work with [a modified version of CNC-sphere-o-bot](https://github.com/klalle/CNC-sphere-o-bot_Ramps_1.4) that I run on an Arduino with Ramps 1.4 shield. 
See tutorial etc [here](https://wiki.evilmadscientist.com/The_Original_Egg-Bot_Kit)

I modified the files
- ebb_serial.py
    - to also look for Arduino Mega (CH340-clone)
    - to increase serial baudrate to 115200
- eggbot_conf.pu
    - to make it work with 32 microstep (all three jumpers with DRC8825)
    - make sure this matches arduino serial.begin in arduino code!

## Install windows:
1. install [inkscape 0.92](https://inkscape.org/release/0.92.4/windows/) 
2. copy the files in the /extensions directory to: `C:\Program Files\Inkscape\share\extensions` (could be `Program Files (x86)`)
3. unzip the [EggBotExamples_v281](EggBotExamples_v281.zip) and open one of those in inkscape (they are just downloaded from the [wiki](https://wiki.evilmadscientist.com/Installing_software))
    - it contains a `EggBotTemplate.svg` that you can use to create your own!
4. Extensions/EggBot/EggBot controll - just follow the [wiki tutorial](https://wiki.evilmadscientist.com/Making_your_first_plot)



EggBot
======

*_Software for The Original EggBot_*

This is a repository for software to drive The Original EggBot, by Evil Mad Scientist Laboratories. More information at http://www.egg-bot.com/

Code here includes the extensions for Inkscape, firmware for the EiBotBoard (AKA "EBB", or EggBotBoard), and example plot files. All code is designed to work on Mac, Windows and Linux.

The latest version of the code is labeled version 2.8.1. New Mac and Windows installers have been released. Manual install is available for Linux (as well as Mac or Windows).


----

This codebase was historically hosted at: https://code.google.com/p/eggbotcode/

Extended documentation available at: http://wiki.evilmadscientist.com/eggbot

------- from release page on original github:

from the releases page: https://github.com/evil-mad/eggbot/releases

Installing this software:
Links to installer applications and instructions are maintained at our wiki, and summarized below.

Please see the notes below about each operating system. We recommend all users to also download the EggBot Example set ( EggBotExamples_v281.zip ), linked in the assets below.

Mac (macOS 10.7-10.14)
Download the Mac install disk image, EggBot.Mac.Bundle.dmg, linked in the assets below. This disk image contains XQuartz and a copy of Inkscape 0.92, modified to include the EggBot software. Run the XQuartz installer, and then copy the included copy of Inkscape to your Applications folder.

Note for AxiDraw users: If you plan to use use both AxiDraw and EggBot, we recommend that you install this version of Inkscape, and then manually install the AxiDraw extensions into the same copy of Inkscape. (Please contact technical support if you need pointers to links or other assistance with this process.)

Manual install for Mac (macOS 10-7-10.14)
If you are unable to use the disk image, you can also install the Inkscape extensions manually. Download and install XQuartz and Inkscape 0.92.2. Launch Inkscape to verify that it opens. Then, download and unzip EggBot_extensions_v281.zip, linked in the assets below. Copy the contents of that folder (20 files and one subfolder) into your Inkscape extensions folder, and then restart Inkscape.

Your Inkscape extensions folder is located at: /Applications/Inkscape.app/Contents/Resources/share/inkscape/extensions/
To open this folder, select "Go to Folder..." Go in the Finder, and paste the location of that folder.

Mac (macOS Catalina 10.15)
This is an early release version. We do not recommend that you use Inkscape 1.0 unless you are on Catalina. Save your work early, and save often.

An installer with simpler instructions is available by request from http://shop.evilmadscientist.com/contact

Download Inkscape 1.0 (beta) for Mac from here

Open that DMG file, copy Inkscape.app from there to your main Applications folder.

Open Inkscape, and verify that it opens correctly. Do not skip this step.

Download and unzip the EggBot software from this release, eggbot-inkv1r2.zip

Copy the contents of that folder (15 files and two subfolders) into your Inkscape extensions directory, found at: /Applications/Inkscape.app/Contents/Resources/share/inkscape/extensions

Restart Inkscape.

Windows
First, download and install Inkscape 0.92.4.

Then, download and run the windows installer program, EggBot_281_r1.exe, linked in the assets below.

Manual install for Windows
If you are unable to use the installer, you can also install the Inkscape extensions manually. Download and install Inkscape 0.92.4. Then, download and unzip EggBot_extensions_v281.zip, linked in the assets below. Copy the contents of that directory (20 files and one subdirectory) into your Inkscape extensions directory, and then restart Inkscape.

Typically, your extensions directory is located at:
C:\Program Files\Inkscape\share\extensions\ or
C:\Program Files (x86)\Inkscape\share\extensions\

Linux
Install and launch Inkscape 0.92. Then, download and unzip EggBot_extensions_v281.zip, linked in the assets below. Copy its contents into your Inkscape extensions directory and relaunch Inkscape.

To find your extensions directory within Inkscape, open Edit > Preferences from the menu, select the System entry. It should list the location of your User extensions directory.

You may also need to add your user name to the dialout group in order to access the USB port. Please see:
https://wiki.evilmadscientist.com/Installing_software#Linux

Firmware Update
A firmware update, to EBB firmware v 2.6.5 is recommended for all EggBot machines, if you currently have older firmware installed. You can check which version you have by using the "Version" tab in the software.

Mac users: Download Firmware_v265_Mac.zip, and run it with EggBot connected to your computer via USB.
Windows users: Download and run Firmware_v265_Win.zip, and run it with EggBot connected to your computer via USB.
Linux users: Please follow the directions here, using the attached file Firmware_v265_Raw.zip.

