# Awesome-Splatoon3-Hacking
repo containing resources to learn splatoon 3 hacking/modding

THIS REPO IS A HUGE W.I.P. Its my side side project when i literally have nothing else to work on

# Getting Started
You're gonna need a modded switch unless you would rather use an emulator. Tutorials can be found here. If you're modding a switch with a copy of Splatoon 3 already on it, good for you. If you're modding a switch with no copy of Splatoon 3 I reccomend buying a legit copy. If you're using an emulator, follow the link to setting up an emulator. It will show you how to get games.
- [Setting up an emulator + Game](https://github.com/Abd-007/Switch-Emulators-Guide/blob/main/README.md)
- [Hacking your switch](https://rentry.org/SwitchHackingIsEasy)

# Essentials
These are programs you should get to help you on your hacking journey. These are all for game modding and NOT for hacking your switch and setting up custom firmware (CFW). For a guide on setting up your switch with CFW, see above section.

- [Flexlion Mod Menu](https://flexlion.github.io/)
- [Splatoon 3 Save Editor (from flexlion)](https://flexlion.github.io/saveeditor.html)
- [Switch Toolbox](https://github.com/KillzXGaming/Switch-Toolbox)
  - [Visual Studio (for compiling, not reccomended for beginners, completely optional)](https://visualstudio.microsoft.com/)
- [7-Zip](https://www.7-zip.org/)

Below are sub-sections for programs that are specific to replacing certain aspects of the game. ***This is not a list of everything you can mod. Just a list of what mods require other programs.***

### Texture Replacement
- Hex Editor. Any hex editor will do. Personally, I use [HxD](https://mh-nexus.de/en/)
- Image Editor (Duh)

### Model Replacement
As of now, Splatoon 3 model replacement is not possible. The encryption on the models hasnt been cracked yet but as more nintendo games start to use the same encryption, I'm sure its just a matter of time. For now, here is an incomplete list on what you WILL need because I cannot predict the future
- [Blender](https://www.blender.org/) or some other 3D Editor

### Text Replacement
- [Kuriimu](https://github.com/IcySon55/Kuriimu) or [Kuriimu 2](https://github.com/FanTranslatorsInternational/Kuriimu2)
Kuriimu 2 is a more permanant, install while Kuriimu is a lighter, portable solution.

# Dumping romfs
### Emulator
(Make sure you have any updates/DLC you want installed as an NSP) Right click the game and click "Dump RomFS"

### Switch
Use [NX Dump Tool](https://github.com/DarkMatterCore/nxdumptool?scrlybrkr=c562aa65) to dump the romfs of the game

# How to use mods
Before you create your first mod, you need to learn how to actually install them. Open the root of your SD card (for emulators go to the root of your virtual sd card) 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/4b9f7abb-1085-4121-bbbb-ade78938816b)

Open the atmosphere folder. Create a folder called `contents` this folder will be where we store our mods. Atmosphere has a built in tool called LayeredFS that replaces game files when booting up the game.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/67c2034b-5030-4bc9-bdc7-7827703a3056)

To start, inside the contents folder, make a folder called `0100C2500FC20000` this is the game ID for splatoon 3. If you have mods for other games, you would make more folders with those game IDs. 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1e734bc1-00da-46b2-b9c0-45f03f49804b)

Now open the game ID folder and make a folder called `romfs` if you havent caught on already, we are remaking the directory for the game. However when we install mods, we only re-create directories that are realitive to the mod files. Most of the time this is already done for you. For now lets set up flexlion and some other mod that replaces a texture or something. Go back the the SD card root and open the flexlion rar file and drag both folders to the root of the sd card from 7-Zip. This will automatically put all the files where they need to be.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fa9e5974-2c8f-4f7b-a81e-55c6e1ed08a7)
