# Awesome-Splatoon3-Hacking
repo containing resources to learn splatoon 3 hacking/modding

THIS REPO IS A HUGE W.I.P. Its my side side project when i literally have nothing else to work on

This will not teach you to use mods/hacks online as that is unsafe. There might be a section to using camera hacks in battle replays later but thats it ****DO NOT USE ANY OF THIS ONLINE. MAKE SURE TO SET UP YOUR HACKED SWITCH PROPERLY****

# Getting Started
You're gonna need a modded switch unless you would rather use an emulator. Tutorials can be found here. If you're modding a switch with a copy of Splatoon 3 already on it, good for you. If you're modding a switch with no copy of Splatoon 3 I reccomend buying a legit copy. If you're using an emulator, follow the link to setting up an emulator. It will show you how to get games.
- [Setting up an emulator + Game](https://github.com/Abd-007/Switch-Emulators-Guide/blob/main/README.md)
- [Hacking your switch](https://rentry.org/SwitchHackingIsEasy)

# Essentials
These are things you need get to help you on your hacking journey. These are all for game modding and NOT for hacking your switch and setting up custom firmware (CFW). For a guide on setting up your switch with CFW, see above section.

- [Flexlion Mod Menu](https://flexlion.github.io/)
- [Splatoon 3 Save Editor (from flexlion)](https://flexlion.github.io/saveeditor.html)
- [Switch Toolbox](https://github.com/KillzXGaming/Switch-Toolbox)
  - [Visual Studio (for compiling, not reccomended for beginners, completely optional)](https://visualstudio.microsoft.com/)
- [7-Zip](https://www.7-zip.org/) I would highly reccomend that you set 7-Zip as your main archiving app so it will open .zip files by default
- [A Full Splatoon 3 Save](https://ptb.discord.com/channels/410208534861447168/830855276437438485/1081218616734793738) (you can skip this if your save already has everything you want AND you know how to export the save as a file using EdiZon) if you cant get to the file, you need to join the [Ryujinx discord server](https://discord.gg/ryujinx) to get it even if you arent using Ryujinx. It will work on both an emulator and the switch.

Below are sub-sections for programs that are specific to replacing certain aspects of the game. ***This is not a list of everything you can mod. Just a list of what mods require other programs.***

### Texture Replacement
- Hex Editor. Any hex editor will do. Personally, I use [HxD](https://mh-nexus.de/en/)
- Image Editor (Duh)
- [Blender](https://www.blender.org/) to check how the texture looks on the model

### Model Replacement
As of now, Splatoon 3 model replacement is not possible. The encryption on the models hasnt been cracked yet but as more nintendo games start to use the same encryption, I'm sure its just a matter of time. For now, here is an incomplete list on what you WILL need because I cannot predict the future
- [Blender](https://www.blender.org/) or some other 3D Editor

### Text Replacement
- [Kuriimu](https://github.com/IcySon55/Kuriimu) or [Kuriimu 2](https://github.com/FanTranslatorsInternational/Kuriimu2)
Kuriimu 2 is a more permanant, install while Kuriimu is a lighter, portable solution.

### Audio Replacement
- [Looping Audio Converter](https://github.com/libertyernie/LoopingAudioConverter)
- [Citric Composer](https://gota7.github.io/Citric-Composer/)
- [Automatic BARS Patcher](https://github.com/ic-scm/automatic-bars-patcher) or [Online BARS Patcher](https://smashcustommusic.net/onlinetools/bars-patcher/)
- [Foobar2000](https://www.foobar2000.org/) + [VGMStream](https://www.foobar2000.org/components/view/foo_input_vgmstream)
- Audio Editor. I use [Audacity](https://www.audacityteam.org)

# Dumping romfs
### Emulator (Beginner reccomended)
(Make sure you have any updates/DLC you want installed as an NSP) Right click the game and click "Dump RomFS" **Make sure to remember where you dumped these files or put them in a place you will remember.**

### Switch (Not for beginners)
Use [Nx Dump Tool](https://github.com/DarkMatterCore/nxdumptool/releases/tag/v1.1.15) to dump the romfs of the game

you can find a tutorial on how to use NX Dump Tool [here](https://suchmememanyskill.github.io/guides/switchdumpguide/)

# Exporting, Editing, and Importing Save Files
First ya gotta obtain a save file. you can get your own save file to hack **OR** download the one in the [essential downloads](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#essentials)

If you're going to use your own save file [download the EdiZon NRO file](https://github.com/WerWolv/EdiZon/releases/tag/v3.1.0)

Once you download, visit [this tutorial](https://www.cfwaifu.com/edizon-saves/) for a full setup process

Go to [The Splatoon 3 Save Editor](https://flexlion.github.io/saveeditor.html) to change (almost) anything about your save and then redownload it (rename the new save file back to `save.dat` if it was changed)

To import it back to splatoon 3, refer to the second part of the tutorial above

# How to use mods
Before you create your first mod, you need to learn how to actually install them. Open the root of your SD card (for emulators go to the root of your virtual sd card) 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/4b9f7abb-1085-4121-bbbb-ade78938816b)

Open the atmosphere folder. Create a folder called `contents` this folder will be where we store our mods. Atmosphere has a built in tool called LayeredFS that replaces game files when booting up the game.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/67c2034b-5030-4bc9-bdc7-7827703a3056)

To start, inside the contents folder, make a folder called `0100C2500FC20000` this is the game ID for splatoon 3. If you have mods for other games, you would make more folders with those game IDs. 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1e734bc1-00da-46b2-b9c0-45f03f49804b)

Now open the game ID folder and make a folder called `romfs` if you havent caught on already, we are remaking the directory for the game. However when we install mods, we only re-create directories that are realitive to the mod files. Most of the time this is already done for you. For now lets set up flexlion and some other mod that replaces a texture or something. Go back the the SD card root and open the flexlion rar file and drag both folders to the root of the sd card from 7-Zip. This will automatically put all the files where they need to be.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fa9e5974-2c8f-4f7b-a81e-55c6e1ed08a7)

Flexlion is now fully installed! Now lets get a mod to go with it

Head over to [Splatoon 3 Mods on Gamebanana](https://gamebanana.com/mods/games/15056) to get some mods. 

Here is not only a shameless self promotion but also [a good starting mod](https://gamebanana.com/mods/439151) 

Download the file titled `Comet Range Blaster` and ignore the download called `Source`. Source just includes the source files i used to make the mod and decided to upload as well. They are not usually submitted with the mod but i figured they migght be useful to someone? idk

Inside the zip file, go to the `romfs` folder inside the `Comet Range Blaster` folder. Now go to your Splatoon 3 game ID folder on your SD card and drag the `romfs` folder from the 7-Zip window on to the `romfs` folder in your SD card.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3ae70e5c-5905-411b-b252-b177e49fec57)

Again, this will do all the replacing automatically even if you already have other mods in there.

Now just eject the SD card, put it into your switch, and launch into Atmosphere CFW again. Refer to [this guide](https://rentry.org/EristaEmuNAND#step-4) if you forgot how to do that

Looks good! Now that you know how to install mods, lets look at how to make them now. I'm going to walk you thorugh making a basic UI image replacement mod

# File Types. Just for future reference
You might be wondering why splatoon 3 only uses `.zs` files inside the romfs folder. ZS is actually short for ZSTD Compression and all that does (that we care about) is add `.zs` to the end of files so the real file type is always behind that. Below are all the other file formats that you can find in the files. Some files are not documented here yet because i dont have the knowledge about them

- `.zs` ZSTD compression used throughout the game files.

- `.bfres` 3D model file containing Models, Textures, Animations, Materials and more. as of now, the encryption keeps us from being able to replace everything besides textures.

- `.pack` Quite literally a package containing many other files. There is really only 1 .pack file that we will go through because it controls most of everything. but that's for later. Usually contains game parameters

- `.sarc` most .sarc files are the language files located in /Mals. Usually contains Message Binary Text files (.msbt) 
  - `.msbt` Contains text that the game uses for each language file. Can be opened in toolbox but needs another program like Kuriimu to be able to edit and save

- `.bfarc` File containing font files located in /Font (they can be ripped and installed like normal fonts too)

- `.bgyml`, `.gyml`, `.byml`, Types of YAML files. Usually contain defining properties.

- `.bntx` Contains an image(s). Most are found in /UI/Icon.

- `.blarc` Layout file that tells the game how to display UI elements (contains a .bntx file for textures).
  - `.bflyt` Part of the layout that tells the game how and where to place/animate UI images on screen
  - `.bflan` Animation file for layout file

- `.bars` File containing game audio. Not usable in switch toolbox but still editable with other programs but we will get to that later.
  - `.bwav` Binary WAV file. Usually nest inside a .bars file but can also be found in /Sound/Resource/Stream.
  

# Your First Mod (Tutorial)

Please ignore the inconsistency of the OS in the screenshots. Some of this was made on my school laptop that administration refuses to upgrade to windows 11

Go to wherever your romfs dump is. Open the `UI` folder and the `Icon` folder. you should now see a lot of folders. Here is an outline of them

![Screenshot 2023-05-10 125139](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/14ef08db-3caf-482f-bf14-b7f8dcd68ff4)

Lets make a badge and a banner mod. To start, lets find the ones we want to replace starting with the badge folder

This may look impossible to search through but its quite easy. Once you get more familliar with everything you'll be able to actually read these names and figure out what it is without even opening it. For now, lets just export all of them as png files so we can decide which one we want to editit

1. Open Switch Toolbox
2. Go to Tools > Batch Export Textures (All Supported Formats)
3. Navigate to your romfs directory and then navigate back to `UI/Icon/Badge` all from the pop up window.
4. `Ctrl` + `A` to select all the files
5. Press Enter
6. Now navigate to an easy to find directory and make a new folder. What this is telling the program to do is to export all the textures we selected previously into wherever your easy to find directory is that you chose. For me, I just made a new folder inside my Documents folder to store all the images.
7. Press Enter
8. Select Portable Graphics Network if it isnt selected by default.
9. Uncheck the top 3 options but keep the bottom one checked

<img width="182" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e755ec24-e3f1-4c76-980d-d7d5fd7174bd">

Click Ok and wait for it to finish. Its going to look like its having a seizure but thats just it opening and closing a progress bar window for every single texture it exports.

Now go to the place you exported them to. You should see all the badge icons in the game. For this tutorial, we're going to select `Badge_Mission_Lv00` because im pretty sure everybody has that badge

10. Open the badge image in a photo editing program of your choice. I'm using Adobe Photoshop 2023. The reason we cant just _replace it_ with any other image is because the image needs to be the exact same pixel size.
11. Make any edits you want or fit an image of your choice in that space. You can literally do anything as long as you dont change the image dimensions. You can even replace it with an image of another badge you want. Or you can go here to get some custom badges from [this website](https://seymourschlong.github.io/splashtags/) if you know how to get the images from the website page source
12. Save your finished image as a png.
13. Find the name of the badge you replaced in the badge folder in your romfs dump.

<img width="200" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/84ccb7e9-afe1-4290-be90-4874dcee39b1">

14. Open the badge file in Switch Toolbox by dragging and dropping it.
15. Open the album icon by clicking the `+` next to it (if there is no plus next to it the double click)
16. Click the image that appears

<img width="662" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/6d590fdd-1d92-4c75-a38b-7d6c1d81c2ba">

17. Right click the image in the heriarchy and select `Replace`

<img width="218" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b7772570-915d-49dd-bdc1-2a7582df1883">

18. Navigate to where you saved the custom badge and select it.
19. In the new options window, change the format to `B8_G8_R8_A8_UNORM` I would reccomend alternating between all the formats to see which one fits best. In my case, this format gives a softer edge as well as an alpha channel and good colors. Select the format box and use the arrow keys to quickly alternate.
20. Click Ok
21. Hover over `Use SRGB` on the right and click the dropdown to change it from false to true

<img width="266" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/8340761b-601c-4b33-a6a6-ed687008599a">

22. Click the save icon in the top left 

<img width="215" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/74b2edd6-4fdd-4433-899b-0b4396c30e06">

23. Click yes to the windows that says "Compress file with ZSTD?"

The file has now replaced the one you originally opened in toolbox. Go back to the badge folder in your romfs dump and find the file you just replaced 

<img width="200" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/84ccb7e9-afe1-4290-be90-4874dcee39b1">

TIP: You can actually see where the file saved via the notification that pops up when you perform a successful file save
  
<img width="305" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/a711d13f-faad-4250-930a-5d1997bb52a2">

24. Copy the file and go to the game ID folder on the sd card (SD/atmosphere/contents)
25. Enter the romfs folder

Steps 26 - 28 can be skipped if you previously downloaded my Comet Range Blaster mod or any other mod that changes UI textures

26. Make a folder called `UI`
27. Inside that folder, make a folder called `Icon`
28. Inside that folder, make a folder called `Badge`
29. Paste the file inside the `Badge` folder

You just made a mod to replace that badge! As you can see, LayeredFS replaces only the files given to it meaning you need to recreate the directory for any files you want to replace in romfs. If you're up for a challenge, try to make a mod that replaces a banner. It's the same process but different folders and images. Remember tha banner folder is called `Npl`

# Replacing Model Textures
Lets do one more harmless mod before we get into the fun stuff.

1. Go into /Model and search for "Wmn". this will filter all results to only show you model files for main weapons

However, these arent images so we cant use our previous method for trying to figure out which is which although soon enough you'll have all the main, sub, and special internal names memorized. For now here is a list on which is which. This is also the order they should appear in your files

This list is as of Fresh Season 2023

`Blaster_Coop` Grizzco Blaster

`Blaster_Light` Rapid Blaster + Rapid Blaster Pro

`Blaster_Light_Cstm01` Rapid Blaster Deco

`Blaster_LightShort` Clash Blaster

`Blaster_LightShort_Cstm01` Clash Blaster Neo

`Blaster_Long` Range Blaster

`Blaster_Middle` Blaster

`Blaster_Short` Luna Blaster

`Blaster_Short_Cstm01` Luna Blaster Neo

`Brush_Mini` Inkbrush

`Brush_Mini_Cstm01` Inkbrush Nouveau

`Brush_Normal` Octobrush

`Charger_Coop` Grizzco Charger

`Charger_Keeper` Goo Tuber

`Changer_Light` Bamboozler 14 Mk I (my beloved)

`Charger_Long` E-Liter + E-Liter Scoped

`Charger_LongB` Splatoon 2 E-Liter (For Amiibo)

`Charger_NormalT` Splat Charger

`Charger_NormalT_Cstm01` Zekkofin Charger

`Charger_Pencil` Snipewriter 5H

`Charger_Quick` Squiffer

`Maneuver_Dual` Dualie Squelchers

`Maneuver_Gallon` Glooga Dualies

`Maneuver_NormalT` Splat Dualies

`Maneuver_Short` Dapple Dualies

`Maneuver_Short_Cstm01` Dapple Dualies Nouveau

`Maneuver_Stepper` Dark Tetra Dualies

`Roller_BrushNormal` Splatoon 2 Octobrush (For Amiibo)

`Roller_Compact` Carbon Roller

`Roller_Compact_Cstm01` Carbon Roller Deco

`Roller_Heavy` Dynamo Roller

`Roller_Heavy_Cstm01` Gold Dynamo Roller (Not Released)

`Roller_Hunter` Flingza Roller

`Roller_NormalT` Splat Roller

`Roller_NormalT_Cstm01` Krak-On Splat Roller

`Roller_Wide` Big Swig Roller

`Saber_Coop` Grizzco Splatana

`Saber_Lite` Splatana Wiper

`Saber_Normal` Splatana Stamper

`Shelter_Compact` Undercover Brella

`Shelter_Coop` Grizzco Brella

`Shelter_Normal` Splat Brella

`Shelter_Wide` Tenta Brella

`Shooter_Blaze` Aerospray MG

`Shooter_Blaze_Cstm01` Aerospray RG

`Shooter_Expert` Splattershot Pro

`Shooter_Expert_Cstm01` Forge Splattershot Pro

`Shooter_First` Splattershot Jr.

`Shooter_FirstCstm01` Custom Splattershot Jr.

`Shooter_Flash` Squeezer

`Shooter_Gravity` .52 Gal

`Shooter_Heavy` .96 Gal

`Shooter_Heavy_Cstm01` .96 Gal Deco

`Shooter_Long` Jet Squelcher

`Shooter_Long_Cstm01` Custom Jet Squelcher

`Shooter_Msn0Lv0` Hero Shot (All 3 Phases)

`Shooter_Normal` Splatoon 1 Splattershot (For Amiibo)

`Shooter_NormalB` Splatoon 2 Splattershot (For Amiibo)

`Shooter_NormalT` Splattershot

`Shooter_QuickLong` Splattershot Nova

`Shooter_Quickmiddle` N-Zap 85

`Shooter_QuickMiddle_Cstm01` N-Zap 89

`Shooter_RvLv0` Rival Octolong Octoshot (Hero Mode)

`Shooter_Short` Sploosh-o-Matic + Splash-o-Matic

`Shooter_Short_Cstm01` Sploosh-o-Matic Neo

`Shooter_Short_Cstm11` Splash-o-Matic Neo

`Shooter_Triple` L-3 Nozzlenose

`Shooter_Triple_Cstm01` L-3 Nozzlenose D

`Shooter_TripleMiddle` H-3 Nozzlenose

`Slosher_Bathtub` Bloblobber

`Slosher_Coop` Grizzco Slosher

`Slosher_Diffusion` Tri-Slosher

`Slosher_Diffusion_Cstm01` Tri-Slosher Nouveau

`Slosher_Launcher`Sloshing Machine

`Slosher_StrongT` Slosher

`Slosher_StrongT_Cstm` Slosher Deco

`Slosher_Washtub` Explosher

`Spinner_Downpour` Ballpoint Splatling

`Spinner_HyperT` Hydra Splatling

`Spinner_QuickT` Mini Splatling

`Spinner_QuickT_Cstm01` Zink Mini Splatling

`Spinner_Serein` Nautilus 47

`Spinner_StandardT` Heavy Splatling

`Stringer_Coop` Grizzco Stringer

`Stringer_Normal` Tri-Stringer

`Stringer_Short` REEFLUX-450

Would you believe me if I said that took 45 minutes to type out

2. Choose your favorite weapon and drag it into toolbox
3. Open the file dropdown and the textures dropdown

<img width="188" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/5d6ea7b9-787b-4434-b756-a1daef67d96a">

For now, lets just modify the base image texture Alb. If you wanna learn about all the maps, I've made a list below this. I wouldent reccomend trying to mess with these textures yet so this is another list thats just here for future reference. Just skip to below the list if you dont care right now. 

`Alb - Albedo` Base image texture. Can also be called `Diffuse`, `Diff`, or `Dif`

`Mlt` Also a base image texture **Not to be confused with Mtl textures**

`Tcl - Team Color` An image mask that tells specific parts of the model to be the ink color of the team and how much

`Ao - Ambient Occlusion` Adds detail/shadows to base textures **Not to be confused with the purpose and functionality of Nrm textures**

`Mtl - Metalness` An image mask that tells specific parts of the model to be matalic and how much

`Rgh - Roughness` An image mask that tells specific parts of the model to have a specified roughness value

`Nrm - Normal Map` Adds details to a model's surcace using vectors extracted from the image for very fine details without adding model geometry. They also look very pretty

`2cl - Ink Damage Effect` This is used to tell the game where on the model to display the enemy ink material when damage is taken

`Mfk - Secondary Normal Map` A very rare map to see paired with a model. This acts as even finer details to the model and very annoying to work with.

`Opa - Opacity` Used to set opacity values to specific parts of the model

`Emm - Emission` An image mask that tells what parts of the model need to have light emission and how strong

`Trm - Transmission` Used to emulate a subsurface scattering effect on a model. usually best to not mess with these

`Thc - Thickness` Helps make the transmission look better. Always paired with a Trm texture

`Hlt / Mac - Highlight` Used to make something very shiny.

`Rft - Lightwarp` Emulates a [Frensel Effect](https://www.3drender.com/glossary/fresneleffect.htm#:~:text=Fresnel%20Effect%20(pronounced%20"fre-,depends%20on%20the%20viewing%20angle.)) as well as the color of it

`Fxm - Effect Mask` Used to mask various material specific effects.

`Hlm - Lightwarp Effect Mask` Used to mask a lightwarp texture

`Mlta / Mltb - Special Effects` Can be used for anything. Nothing specific.

`Mai - Skin Mask` Image mask usually used to define what part of the model is skin and what is not.

Source : [PastaOwO's Squidnodes Materials and Textures Wiki](https://github.com/PastaOwO/Squidnodes/wiki/Materials-and-Textures?scrlybrkr=c562aa65)

4. Open the `Models` folder and export the model as a .dae (if there are multiple models, export all of them as .dae)

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c783d707-358c-485a-ad5c-c84c2c3224a6)

5. Navigate to a directory you will remember. Make a new folder there to place the files in. Save inside that folder

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1e12ba1b-f9f1-4d7b-b2c6-cc567fa20e15)

6. Toggle Use Old Exporter and untoggle Use Texture Channel Swaps

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/8e74a838-d132-44a1-a4db-7b31d708d17a)

7. Open Blender and import the .dae (after deleting the default scene objects

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e7acea74-9225-4698-a9d9-38c95b595419)

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b580dc9e-9320-4048-bdab-3469931ad9f8)

8. Adjust the edges of the editors to your liking. Then change the outliner editor to a shader editor

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/0f00fe25-9aa0-4d0d-a331-c2d539c90690)

9. Set the `Specular` value of the principled BSDF node to `0.5` 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/19224fec-741a-462c-b4c7-4b49e42b4e2d)

10. For each of these image textures that your model came with, drag and drop them into the shader editor one by one. `Alb`, `Mtl`, `Nrm`, `Rgh`. these are just the bare basics to give us a preview

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/7b6c3125-4b80-4cf7-a7ec-fd95d168ce8d)

11. Use `Shift` + `A` and type in "nm" or "normal map' into the text box to make a Normal Map node

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/7c872174-9f4d-484c-93bf-098992c714ab)

12. This isnt a Blender tutorial so just make sure your node setup looks like this. the only things you need to look for are the things circled and the node connections

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/a111b6b0-cac8-46c6-be8c-6186846811f0)

