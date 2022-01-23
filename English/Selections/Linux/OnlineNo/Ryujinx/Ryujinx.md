# You've chosen: Ryujinx

This guide will go through all the essential steps required to get Ryujinx emulator set up. We're going to split this guide into required and optional sections. Parts that are required to get the emulator playing your game of choice, and parts that may enhance the experience to some degree. 

## Please do not skip over the essential parts of the guide

### Method 1 (Installer (Recommended)):

#### If you want to have a portable install, click [this](#Method-2-Portable)

*This method uses a bash script written by edisionnano. All credits for this method go to their team.*

To start, you're going to need to open your terminal. Then paste this command and execute it in the terminal: ` bash -c "$(curl -s https://raw.githubusercontent.com/edisionnano/Pine-jinx/main/pinejinx.sh)"` 

Once you see this option, press '1' on your keyboard and hit enter:
![Once you see this option, press '1' on your keyboard and hit enter](![image](https://user-images.githubusercontent.com/81475204/149823010-6c7c8ae9-12e4-4338-acab-d6baed89d21a.png)

Then press 'y' when it asks for game mode (only select 'N' if you have a custom kernel)
![image](https://user-images.githubusercontent.com/81475204/149822991-dc5d532a-8951-4180-b150-d4083c0d01b5.png)

When you are given this option, press the number for the graphics card vendor you're using (1 for Nvidia, 2 for AMD or Intel)
(![image](https://user-images.githubusercontent.com/81475204/149823182-7a8bf9e6-fd5c-4754-8fa6-536c517382c4.png)

Then it'll ask to disable console window (Press 'Y' if you don't want to see debug logs or 'N' if you prefer to see the logs)

*Placeholder for pinejinx alias question*

Now that the script as finished installing, you should have Ryujinx added to your start menu
![image](https://user-images.githubusercontent.com/81475204/149824494-85204931-d660-44d1-abd7-daae644d32f4.png)

*Method 1 install complete, click [This button](#Keys-and-firmware) to go to the next step*

* * *

### Method 2 (Portable):

*This method is taken directly from the Ryujinx website*

To start, you need to go to https://ryujinx.org/download and download the linux build on this page. You should have a tar.gz file downloaded. 

You can extract it by opening a terminal in the folder where Ryujinx was downloaded to (or CDing over to the folder in question) and then paste `tar –xvzf ryujinx-versionNumber.tar.gz`. This will extract to the same folder the tar file is pasted in.

Alternatively, if your distro supports it you can extract it using the archive manager GUI (Debian-based distros have these built in usually).

Now, navigate to the publish folder that was extracted from Ryujinx and it should look something like this: ![image](https://user-images.githubusercontent.com/81475204/149984230-5164db58-d848-44e5-8a34-564ebee9979e.png)

Since you've opted for an entirely portable install, you'll need to create a new folder titled 'portable' ![image](https://user-images.githubusercontent.com/81475204/149984709-724b8ab9-e9da-41e9-868d-a3f9a7f4d633.png)

Now you've done that, open a terminal in the publish folder and paste in `./Ryujinx`

On startup, you should be met with an error that looks like this. Don't press anything and now is a good time to check the logs in the terminal. In the launch mode box, it should say `portable` like this: ![image](https://user-images.githubusercontent.com/81475204/149985172-a42ccaa0-bb58-4945-9c0d-ea41e1470e80.png)

(If it doesn't, close Ryujinx and try again. Make sure that 'portable' is all lower case)


## Keys and firmware

### If you want to do all this manually with no extra tools, you must follow [this guide](https://github.com/Ryujinx/Ryujinx/wiki/Ryujinx-Setup-&-Configuration-Guide#initial-setup---placement-of-prodkeys) and find the key files yourself. However, we recommend following the easier method down below. We 

For everyone else, this is a method to make the process a lot easier:

We recommend using [emusak](https://github.com/CapitaineJSparrow/emusak-ui) to download your keys and firmware. This is a free program that can automatically place your keys and download shader caches for games (which is something we'll come to in the optional guide). If you're on debian-based distros (such as mint or ubuntu), it's as easy as grabbing the `.deb` file and running it from here: https://github.com/CapitaineJSparrow/emusak-ui/releases/

If you're on another distro, we recommend reading the install guide on emusak here: https://github.com/CapitaineJSparrow/emusak-ui#Installation

Once you've successfully installed it the way listed for your distro, emusak should be installed to the start menu like this: ![image](https://user-images.githubusercontent.com/81475204/149989142-28e3bb8e-847b-4b9a-9a12-c0c5bb913a9b.png)

Open it and you should be greated with something like this: ![image](https://user-images.githubusercontent.com/81475204/149989316-8bfc56b5-785e-4087-bfe5-1e06e0f12d4e.png)

On the top right, there's a button to add a Ryujinx folder: [add image]

*If you followed the portable install guide, open the `publish` folder where you extracted Ryujinx before*

If you installed Ryujinx using pinejinx, go to ### ADD FILE LOCATION LATER

Once you've done all that, you should be given options to download firmware and keys:

Download the keys first then download the firmware
