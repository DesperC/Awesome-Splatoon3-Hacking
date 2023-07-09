# Awesome-Splatoon3-Hacking
repo containing resources to learn splatoon 3 hacking/modding

THIS REPO IS A HUGE W.I.P. and it is very unfinished. Its my side side project when i literally have nothing else to work on

This will not teach you to use mods/hacks online as that is unsafe. There might be a section to using camera hacks in battle replays later but thats it ****DO NOT USE ANY OF THIS ONLINE. MAKE SURE TO SET UP YOUR HACKED SWITCH PROPERLY****


# Table of Contents
- Getting Started
- Essentials/Requirements
  - Texture Replacement (Old)
  - Texture Replacement
  - Model Replacement
  - Audio Replacement
- Dumping RomFS
  - Using an Emulator
  - Using a Switch
- Exporting, Editing, and Importing Save Files
- How to use/install mods
- File Types. Just for future reference
- Your First Mod (Tutorial)

# Getting Started
You're gonna need a modded switch unless you would rather use an emulator. Tutorials can be found here. If you're modding a switch with a copy of Splatoon 3 already on it, good for you. If you're modding a switch with no copy of Splatoon 3 I reccomend buying a legit copy. If you're using an emulator, follow the link to setting up an emulator. It will show you how to get games.
- [Setting up an emulator + Game] link removed due to piracy
- [Hacking your switch](https://rentry.org/SwitchHackingIsEasy)

# Essentials/Requirements
These are things you need get to help you on your hacking journey. These are all for game modding and NOT for hacking your switch and setting up custom firmware (CFW). For a guide on setting up your switch with CFW, see above section.

- [Flexlion Mod Menu](https://flexlion.github.io/)
- [Splatoon 3 Save Editor (from flexlion)](https://flexlion.github.io/saveeditor.html)
- [Switch Toolbox](https://github.com/KillzXGaming/Switch-Toolbox)
  - [Visual Studio (for compiling, not reccomended for beginners, completely optional)](https://visualstudio.microsoft.com/)
- [7-Zip](https://www.7-zip.org/) I would highly reccomend that you set 7-Zip as your main archiving app so it will open .zip files by default
- [A Full Splatoon 3 Save](https://ptb.discord.com/channels/410208534861447168/830855276437438485/1081218616734793738) (you can skip this if your save already has everything you want AND you know how to export the save as a file using EdiZon) if you cant get to the file, you need to join the [Ryujinx discord server](https://discord.gg/ryujinx) to get it even if you arent using Ryujinx. It will work on both an emulator and the switch.

Below are sub-sections for programs that are specific to replacing certain aspects of the game. ***This is not a list of everything you can mod. Just a list of what mods require other programs.***

### Texture Replacement (Old)
- Hex Editor. Any hex editor will do. Personally, I use [HxD](https://mh-nexus.de/en/)
- Image Editor (Duh)
- [Blender](https://www.blender.org/) to check how the texture looks on the model

### Texture Replacement
- Image Editor (still, duh)
- [Blender](https://www.blender.org/) to check how the texture looks on the model

### Model Replacement
- [Blender](https://www.blender.org/) or some other 3D Editor and good knowledge of how to use it. Model replacement is for people who know how to use the program. basically, 3d model experience required

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

### Emulator (Beginner reccomended) (Required if you arent using switch)
(Make sure you have any updates/DLC you want installed as an NSP) Right click the game and click "Dump RomFS" **Make sure to remember where you dumped these files or put them in a place you will remember.**

### Switch (Not for beginners)
you need Lockpick RCM and Nxdumptool

im not allowed to link LockpickRCM but you can find it so many places here on github. just search it and download te .bin file

then watch[ this video](https://www.youtube.com/watch?v=mKw2ips97og) on how to use it

once you finish that, download [Nxdumptool nro file](https://github.com/DarkMatterCore/nxdumptool/releases)

then watch [this video](https://www.youtube.com/watch?v=BZpK2JT8lcI) on how to use that

only reason i dont explain myself is because this guide is focused on how to mod the game rather than the setup

# Exporting, Editing, and Importing Save Files
First ya gotta obtain a save file. you can get your own save file to hack **OR** download the one in the [essential downloads](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#essentials)

If you're going to use your own save file [download the EdiZon NRO file](https://github.com/WerWolv/EdiZon/releases/tag/v3.1.0)

Once you download, visit [this tutorial](https://www.cfwaifu.com/edizon-saves/) for a full setup process

Go to [The Splatoon 3 Save Editor](https://flexlion.github.io/saveeditor.html) to change (almost) anything about your save and then redownload it (rename the new save file back to `save.dat` if it was changed)

To import it back to splatoon 3, refer to the second part of the tutorial above

# How to use/install mods
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

Again, this will do all the replacing automatically even if you already have other mods in there. It wont overwrite anything unless you have another range blaster mod installed

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

26. Make a folder called `UI`

27. Inside that folder, make a folder called `Icon`

28. Inside that folder, make a folder called `Badge`

29. Paste the file inside the `Badge` folder

You just made a mod to replace that badge! As you can see, LayeredFS replaces only the files given to it meaning you need to recreate the directory for any files you want to replace in romfs. If you're up for a challenge, try to make a mod that replaces a banner. It's the same process but different folders and images. Remember tha banner folder is called `Npl`

# Replacing Model Textures (Old)

I feel like leaving this method in might be useful to someone but now, its outdated. for the in-date tutorial, check here

Lets do one more harmless mod before we get into the fun stuff.

1. Go into /Model and search for "Wmn". this will filter all results to only show you model files for main weapons

However, these arent images so we cant use our previous method for trying to figure out which is which although soon enough you'll have all the main, sub, and special internal names memorized. For now here is a list on which is which. This is also the order they should appear in your files

### [This list is as of Sizzle Season 2023](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#list-of-weapons-as-of-fresh-season-2023)

2. Choose your favorite weapon and drag it into toolbox
3. Open the file dropdown and the textures dropdown

For now, lets just modify the base image texture Alb. If you wanna learn about all the maps, I've made a list below this. I wouldent reccomend trying to mess with these textures yet so this is another list thats just here for future reference. Just skip to below [the list](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#texture-names) if you dont care right now. 

<img width="188" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/5d6ea7b9-787b-4434-b756-a1daef67d96a">

4. Open the `Models` folder and export the model as a .dae (if there are multiple models, export all of them as .dae)

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c783d707-358c-485a-ad5c-c84c2c3224a6)

5. Navigate to a directory you will remember. Make a new folder there to place the files in. Save inside that folder

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1e12ba1b-f9f1-4d7b-b2c6-cc567fa20e15)

### 6. Toggle Use Old Exporter and untoggle Use Texture Channel Swaps

if you're here from the updated texture tutorial, follow along until step 25

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

13. turn on material preview mode

 <img width="229" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/876af7dd-b6c2-43ed-a159-a167b54d5018">


14. Your model may have multiple objects and materials. If so, here is how to assign them correctly (If you dont have multiple materials then skip to step 15)
  - Your model has multiple materials if you see more than 1 prefix in your image texture files. this screenshot shows image texture files with a total of 3 prefixes
  
  <img width="839" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1cbe5a0e-4bc6-498e-837c-91d94427e2b9">
  
  - For each prefix you have, there should also be a material. The material for each prefix should be on its respective object. To view all the objects, pull up the timeline window hiding at the bottom of the screen and change the clock icon to be the one labaled outliner.
  
  <img width="589" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c1c225e1-2f70-44bd-9304-be9c3fce29ee">
  
  - Press `Shift` + `A` to expand everything and locate everything reperesented by a triangle icon. those are your objects. Click on an object and go to the material properties
  
  <img width="950" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/2d8532dd-0bcd-434d-86ac-7c501f78e84b">
  
- Select the material and drag in the image textures which prefixes match the material name. Then repeat above process for each

<img width="482" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fcf60101-03e0-40da-af58-6ac55123bc35">

- Your model could also have multiple models that actually use the same texture but it has a different material. If your image textures only have 1 prefix but some part of your model is still white, then assign the white model(s) the same material as the other model
 
15. Change the properties editor to a UV Editor
 
 <img width="616" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/2ff66f6b-992e-4608-9bda-75b2f4340201">

16. Open the image you want to edit. In this case, we are only editing the Alb image

 <img width="400" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/9b8d0372-5747-47cc-8caf-0badc5a61f48">

17. Back in the viewport, select the model, press `Tab` to switch to edit mode, and press `A` to select all vertecies. Your UV editor should be filled with orange dots and lines

 <img width="860" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b504c7bc-eaee-4cf5-a28a-a565cd0a1fce">

18. In the UV editor, click the UV pannel and select Export UV Layout. You may need to scroll down the menu to see it.

 <img width="395" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/81a2f384-a201-4e3d-8fe2-8ca3d87b298d">

19. For organizational purposes, export the png file to the same place as all your image textures. Make sure to name it something that stands out

20. Open your photo editing program. Import the Alb texture and place the exported UV layout image on top of it. Now we can see how the model displays the texture.

21. Now go crazy. put anything you want on it. Remember not to change the size of the image though.

TIP: Remember to repeat the above process to get the UV layout for **ALL** of the objects that use the same material and put that UV map over the first one. You'll know if multiple objects are using the same material if there is some detail that looks like it should be covered by a UV layout.

22. Once done, hide the UV layout images so they dont appear in the final product. Export it in the same place as the original Alb image to replace it. we wont need it anymore

23. Back in the shader editor, click on the Alb node. then hit `N` to bring up a panel. Go to the `Node` section on that panel. Click the refresh button to refresh the image texture and make sure its to your liking

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/ca50a936-8e3d-460b-b504-b8a09a30255a)

25. Once ready, go back to toolbox and replace the Alb image on the model. The default settings in the window that pops up should be fine

<img width="229" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/dae238af-b5d9-4d09-b7dd-45052ed0588e">

**If you're following along with the new tutorial, return back to that section using [this link](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#9-save-the-bfres-file-using-the-save-icon-in-the-top-left-corner). if you're using this tutoairl because that method diddnt work, ignore this message.

26. Right click the `Textures` folder and click export

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e86377bc-3ea5-4f78-bb49-c98a1943e947)

27. Save it as `textures.bntx` to where your model and textures are

28. In toolbox, go to Tools > Compression > ZSTD > Decompress

29. Find your model in the models forlder and open it

30. Remove the `.zs.dec` in the name so the file extension becomes `.bfres`

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/79dd3b59-aeee-49c5-86a2-efd633ee198d)

31. Save it to where you originally exported the model

32. Open your hex editor. I'm using HxD

33. Drag the `.bfres` file into the hex editor to open it. You should now see a bunch of random characters

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/86474eaf-3767-4eb4-8435-107afaa873be)

34. Do the same for `textures.bntx` it should open in a new tab

35. Go to the `textures.bntx` tab and copy all of it (`Ctrl` + `A` then `Ctrl` + `C`)

36. Go back to the Wmn_Weapon_Name`.bfres` and hit `Ctrl` + `F`

37. Type in "bntx"

38. Click "Search All"

39. We want the line that has "BNTX" in all caps. That should always be the second line

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/f5a733bc-4c1d-4508-9bca-9ce4244b0ffe)

40. Click it to go to it.

41. Click Right before the highlighted portion (42 4E 54 58) right click and click "Paste Write." You should now see a lot of red text.

42. Hit `Ctrl` + `S` to save it. The text should be normal now. You can close the hex editor. (A `.bak` file might have been created. Ignore it)

43. Lets check if it worked. Drag the `.bfres` file into toolbox. If everything worked, you should see your textures on it now.

44. Go to Tools > Compression > ZSTD > Compress

45. Navigate to your folder with the `.bfres` file you just opened and select it.

46. Delete the "td" at the end of `zstd` on the file. it should now read Model_Name.bfres.zs

47. Now navigate to your `romfs` folder for your SD card where you keep mods for the game. Inside your `romfs` location, make a folder called "Model" if it isnt there already.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/780d6b5e-5b70-4076-bce3-c84fd9d0f1b2)
ignore the 485348974563 mods I have in there its not important

49. Save the `.bfres.zs` inside the model folder

50. Boot up the game

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/95cf45d1-afa5-4a15-b22a-21152ccd8e6e)

Awesome! You just finished your own weapon reskin.

# Replacing Textures

**This method is still experimental. if it fails, please refer to the above texture replacement guide in order to replace textures as it is much more reliable but takes a bit longer**

let's make a mod that changes the base texture of your favorite weapon.

1. Start by going into romfs/Model and searching for `Wmn` this will filter results so we only get main weapon models.

if you wanna do a peice of gear instead there are lists for all gear codenames with pictures up until 3.0.0 for now made by my friend John#1878 on discord

[Headgear](https://docs.google.com/document/d/1SaQOljCMUCjGNYzhnbqUHCXR1vrdef67vUVbcv_2Lkg/edit)

[Clothing](https://docs.google.com/document/d/1bIje-QhxGa0EThWjB5V9xj_Jqfj9D8Bjkb-Wu9ruNSg/edit)

[Shoes](https://docs.google.com/document/d/1MwfrztugDbqNlU6S87Oflz-WQrSwxC20zV25aqNwn9k/edit)

### List of weapons as of Sizzle Season 2023

`Blaster_Coop` Grizzco Blaster

`Blaster_Light` Rapid Blaster + Rapid Blaster Pro

`Blaster_Light_Cstm01` Rapid Blaster Deco

`Blaster_Light_Cstm11` Rapid Blaster Pro Deco

`Blaster_LightShort` Clash Blaster

`Blaster_LightShort_Cstm01` Clash Blaster Neo

`Blaster_Long` Range Blaster

`Blaster_Middle` Blaster

`Blaster_Precision` S-Blast 92

`Blaster_Short` Luna Blaster

`Blaster_Short_Cstm01` Luna Blaster Neo

`Brush_Heavy` Painbrush

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

`Maneuver_Dual_Cstm01` Custom Dualie Squelchers

`Maneuver_Gallon` Glooga Dualies

`Maneuver_NormalT` Splat Dualies

`Maneuver_Short` Dapple Dualies

`Maneuver_Short_Cstm01` Dapple Dualies Nouveau

`Maneuver_Stepper` Dark Tetra Dualies

`Maneuver_Stepper_Cstm01` Light Tetra Dualies

`Roller_BrushNormal` Splatoon 2 Octobrush (For Amiibo)

`Roller_Compact` Carbon Roller

`Roller_Compact_Cstm01` Carbon Roller Deco

`Roller_Heavy` Dynamo Roller

`Roller_Heavy_Cstm01` Gold Dynamo Roller (Not Released)

`Roller_Hunter` Flingza Roller

`Roller_NormalT` Splat Roller

`Roller_NormalT_Cstm01` Krak-On Splat Roller

`Roller_Wide` Big Swig Roller

`Roller_Wide_Cstm01` Big Swig Roller Express

`Saber_Coop` Grizzco Splatana

`Saber_Light` Splatana Wiper (Wiper can also be seen in other places named `Saber_Lite` instead)

`Saber_Light_Cstm01` Splatana Wiper Deco

`Saber_Normal` Splatana Stamper

`Shelter_Compact` Undercover Brella

`Shelter_Coop` Grizzco Brella

`Shelter_Normal` Splat Brella

`Shelter_Wide` Tenta Brella

`Shelter_Wide_Cstm01` Sorella Tenta Brella

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

`Shooter_NormalT_Cstm01` Tentatek Splattershot

`Shooter_QuickLong` Splattershot Nova

`Shooter_QuickLong_Cstm01` Anakai Splattershot Nova

`Shooter_Quickmiddle` N-Zap 85

`Shooter_QuickMiddle_Cstm01` N-Zap 89

`Shooter_RvLv0` Rival Octolong Octoshot (Hero Mode)

`Shooter_Short` Sploosh-o-Matic + Splash-o-Matic

`Shooter_Short_Cstm01` Sploosh-o-Matic Neo

`Shooter_Short_Cstm11` Splash-o-Matic Neo

`Shooter_Triple` L-3 Nozzlenose

`Shooter_Triple_Cstm01` L-3 Nozzlenose D

`Shooter_TripleMiddle` H-3 Nozzlenose

`Shooter_TripleMiddle_Cstm01` H-3 Nozzlenose D

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

`Spinner_StandardT_Cstm01` Heavy Splatling Deco

`Stringer_Coop` Grizzco Stringer

`Stringer_Normal` Tri-Stringer

`Stringer_Short` REEFLUX-450

Would you believe me if I said that took 45 minutes to type out

For now, lets just modify the base image texture Alb. If you wanna learn about all the maps, I've made a list below this. I wouldent reccomend trying to mess with these textures yet so this is another list thats just here for future reference. Just skip to below the list if you dont care right now. 

### Texture Names
`Alb - Albedo` Base image texture. Can also be called `Diffuse`, `Diff`, or `Dif`

`Mlt` Also a base image texture **Not to be confused with Mtl textures**

`Tcl - Team Color` An image mask that tells specific parts of the model to be the ink color of the team and how much. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Ao - Ambient Occlusion` Adds detail/shadows to base textures **Not to be confused with the purpose and functionality of Nrm textures**

`Mtl - Metalness` An image mask that tells specific parts of the model to be matalic and how much. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Rgh - Roughness` An image mask that tells specific parts of the model to have a specified roughness value. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Nrm - Normal Map` Adds details to a model's surcace using vectors extracted from the image for very fine details without adding model geometry. They also look very pretty

`2cl - Ink Damage Effect` This is used to tell the game where on the model to display the enemy ink material when damage is taken. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Mfk - Secondary Normal Map` A very rare map to see paired with a model. This acts as even finer details to the model and very annoying to work with.

`Opa - Opacity` Used to set opacity values to specific parts of the model. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Emm - Emission` An image mask that tells what parts of the model need to have light emission and how strong. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Trm - Transmission` Used to emulate a subsurface scattering effect on a model. usually best to not mess with these

`Thc - Thickness` Helps make the transmission look better. Always paired with a Trm texture. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Hlt / Mac - Highlight` Used to make something very shiny. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Rft - Lightwarp` Emulates a [Frensel Effect](https://www.3drender.com/glossary/fresneleffect.htm#:~:text=Fresnel%20Effect%20(pronounced%20"fre-,depends%20on%20the%20viewing%20angle.)) as well as the color of it

`Fxm - Effect Mask` Used to mask various material specific effects. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Hlm - Lightwarp Effect Mask` Used to mask a lightwarp texture. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

`Mlta / Mltb - Special Effects` Can be used for anything. Nothing specific

`Mai - Skin Mask` Image mask usually used to define what part of the model is skin and what is not. Black means 0 intensity, grey means anywhere from 0-1 intensity depending on how dark or bright it is, and white means 1 intensity

Source : [PastaOwO's Squidnodes Materials and Textures Wiki](https://github.com/PastaOwO/Squidnodes/wiki/Materials-and-Textures?scrlybrkr=c562aa65)

2. decompress the file using Tools > Compression > ZSTD > Decompress and save it to a place you can find it.
3. drag the `.bfres` file you just decompressed into toolbox
4. click on the model folder.
5. right click on the model that uses the texture(s) you want to modify
6. export it as `.dae` to the same folder your `.bfres` is in.
7. check `Use Old Exporter` and uncheck `Use Texture Channel Swaps`
8. refer to [this section](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#6-toggle-use-old-exporter-and-untoggle-use-texture-channel-swaps) of the old method because i cant be bothered to explain again.

### 9. Save the .bfres file using the save icon in the top left corner

10. Recompress the file using Tools > Compression > ZSTD > Compress and compress the bfres file
11. remove the "td" at the end of `zstd` to make it just say 'zs' and then save that file to the model folder of your sd card romfs directory.

TIP : You can combine these 2 modding tecniques that you've learned so far to create custom icons and badges for your reskin just like my [Comet Range Blaster mod!](https://gamebanana.com/mods/439151) To learn how to make 2D icons from 3D models, here is a link to a small tutorial inside the repo. (TO BE MADE)

# Replacing Text.
This is how i made my Google Translate Mod. Hours of copying text from the game and putting it through translate a million times. Cant believe im gonna do the same thing for side order

Anyways enough of my crippling anxiety, lets start by [downloading the required editor](https://github.com/DesperC/Awesome-Splatoon3-Hacking?scrlybrkr=c562aa65#text-replacement)

I would reccomend setting Kuriimu as your default .msbt editing program so you dont need to drag the file in the program to open it every time.

1. In your romfs dump, open the Mals folder. i'm assuming youre language is english so we want this file right here

<img width="224" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1d31f2c2-80d4-4efc-9c39-24d676f2721e">

2. Drag the file into toolbox to open it. there are a ton of .msbt files in here so here is a small list of where important ones are as well as important prefixes

any files starting with `msn` or `mission` or any files located inside the `LogicMsg` folder or any files in `CommonMsg/Mission` relate to hero mode

any files starting with `vs` or `versus` or `lobby` relate to multiplayer

you can find the splashtag titles files in `CommonMsg/Byname`

weapon names are in `CommonMsg/Weapon` 

try looking at the glossary file in `CommonMsg/Glossary.msbt` if you want to find names of characters

gear names can be found at `CommonMsg/Gear`

text relating to salmon run is any file that has `Coop` or `LobbyCoop` in the name

if you want to edit what Deep Cut says on the news, search for any files starting with `News`

Toolbox cant edit the msbt files so we need to export them to edit them.

3. Find any `.msbt` files you want. right click on them and click Export Raw Data

<img width="305" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/abb00fc6-c6d7-4173-8fc5-d071411ac62a">

4. Save the file to a place you will remember

5. open Kuriimu then open the .msbt file with Kuriimu by dragging it over

6. click yes to keep a backup. this is very helpful for multiple reasons then just if you need to revert

<img width="295" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/9724c759-6e35-438c-acbb-95893a3eb744">

7. Click this icon here to get a preview inside the text entries

<img width="249" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e6a1cb3c-c657-4cbf-8087-5ecf5f25cfdb">

Dont worry if the entry names are gibberish. We never need to worry about names

remember you can always use these 2 options to find something(s) specific (first one) or find and replace something(s) specific (second one)

<img width="128" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/cf9ac1e0-ef99-4658-8414-9b0b806417db">

8. Once you edit everything you want to edit, do `Ctrl` + `S` to save the file.

9. back in toolbox, right click the file you just exported but now click Replace Raw Data

<img width="349" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/0258b0d8-5105-4fec-bafb-3c6ff27b77dd">

10. Navigate to the `.msbt` file you edited with Kuriimu. You should also see a `.bak` file there. ignore it

11. select the `.msbt` file

12. back in toolbox, double click the file you just replaced to open a preview of it to make sure it has your edits. toolbox can preview msbt files but it cant edit them.

<img width="454" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/11143db9-66b6-47fa-88d8-70a99814a37a">

13. Close the pop up window and save the file 

<img width="142" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c4973c0c-a84e-4e64-ae3f-60f862ef4ff8">

14. Click Yes to the promt

<img width="148" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/f12a659b-2218-4a5a-a392-6499eedb39e9">

15. Copy the `.sarc` file we just edited and navigate to your SD card romfs directory. Make a new folder called Mals and paste the file in there

16. Boot up the game

NOTE: You will need to 

Text editing is one of the simplest but most effective ways of modding in my opinion. I really enjoy making characters just say the dumbest things.

# Editing UI Layouts

Not started yet but you can use when ive already taught you to edit the files in the Layout folder

# Replacing Audio
This is completely optional. If you wanna learn how to actually get into the _hacking_ part of this then skip to the next section. Otherwise follow this tutorial

cant be bothered to write out my own right now. might do this last. for now, refer to [this tutorial](https://gamebanana.com/tuts/15422)

# Custom Kits
Time for your first game hack. Weapon kits are stored in romfs/RSDB/`WeaponInfoMain.Product.GAME_VERSION.rstbl.byml.zs`

Before we get started, here is a list of all the subs and specials that can go on weapons

`SpBlower` Ink Vac

`SpCastle` Kraken

`SpChariot` Crab Tank

`SpEnergyStand` Tacticooler

`SpFirework` Super Chump

`SpGachihoko` Rainmaker

`SpGreatBarrier` Big Bubbler

`SpInkStorm` InkStorm

`SpJetpack` Inkjet

`SpMicroLaser` Killer Wail 5.1

`SpMultiMissile` Tenta Missiles

`SpNiceBall` Booyah Bomb

`SpShockSonar` Wavebreaker

`SpSkewer` Reefslider

`SpSuperHook` Zipcaster

`SpSuperLanding` Splashdown (yes really)

`SpTripleTornado` Tristrike

`SpUltraShot` Trizooka

`SpUltraStamp` Ultra Stamp

Sub Weapons, if there are parenthesis next to a name, that tells you its second name that can be seen in the files on occasion. The second names arent too important i just put them there so you would know.

`Beacon` Beacon (`Flag`)

`Bomb_Curling` Curling Bomb

`Bomb_Fizzy` Fizzy Bomb (`Bomb_Piyo`)

`Bomb_Quick` Burst Bomb (`Bomb_Handy`)

`Bomb_Robot` Autobomb (`Bomb_Robo`)

`Bomb_Splash` Splat Bomb

`Bomb_Suction` Suction Bomb (`Bomb_Hold`)

`Bomb_Torpedo` Torpedo (`Bomb_Tako`)

`LineMarker` Line Marker (`LinMarker`)

`PointSensor` Point Sensor (`MarkingBall`)

`PoisonMist` Toxic Mist (`DevillBall`)

`SalmonBuddy` Lil' Buddy - Needs to be modified if you want to use it on a weapon

`Shield` Splash Wall

`Sprinkler` Take a guess

`Trap` Ink Mine

Alright. Now we can get to editing kits.

1. Open switch toolbox and go to Tools > Compression > ZSTD > Decompress

2. Go to your romfs dump and go inside RSDB. Select `WeaponInfoMain.Product.GAME_VERSION.rstbl.byml.zs`

3. Delete the ".zs.dec" at the end of the file name so you're left with ".bfres" as the extension

4. save the file in a place so it will be easy to find.

5. go to where you saved the file and drag it into toolbox

6. Use [this list](https://github.com/DesperC/Awesome-Splatoon3-Hacking/edit/main/README.md#this-list-is-as-of-fresh-season-2023) again to find your weapon.

7. switch to text editor and hit "Decompile." hit `Ctr` + `F` and type in the weapon codename. dont use any underscores

8. Find the paragraph that looks like this relating to your weapon

<img width="667" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/23a2d883-8a23-4a45-b500-83361f70bc08">

9. The only notable things you can change in this file are:

- Weapon kits

- Weapon Special Points

- What badges you get from getting 4 and 5 star on that weapon

- Weapon UI Values (a.e the game showing you how much range the weapon has)

- Weapon ID. This is a bit more complicated and is explained what it is and how to do later in the guide.

10. Right now, we will only need to look at these 3 lines

<img width="518" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1dce16e1-0f11-4276-9370-b8a132ec3ec4">

Note that this isnt the correct kit for Bamboozler because i have already messed with it. Dosent change the process for changing any weapon kit though

11. Lets replace the special first. Copy the special codename you want from the list above and replace the original special

This is the only part of the line that needs to be fully replaced with your special

<img width="494" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e9e302e7-83bb-4650-9501-d1d57da15a3b">

12. Now do the same thing for the sub weapon. Again this is the only part that should be replaced 

<img width="437" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c8ec91e7-a01a-433f-9461-73ec9a66bcc6">

13. If you feel like it, edit the required amount of special points for the weapon. Setting it to 0 will automatically fill the special meter again after you use it

<img width="143" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/09f8ba82-3738-48f9-aac7-37de715b1366">

Dont worry about the `!l` thats just telling the game that its a Int32 value meaning it can store values up to 2,147,483,647

14. compile it by clicking "Compile" near the top of the window

<img width="297" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/49ec7fbd-24d3-4399-aa9f-9b4e2fa0e226">

15. Now save it with the save icon

<img width="250" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/d1290a51-21b4-438e-b469-b1eec8d5774e">

Finally, we need to recompress it

16. go to Tools > Compression > ZSTD > Compress

17. select the .byml you just saved

18. delete the "td" at the end of the file name so the end of the file reads `.rstbl.byml.zs`

19. navigate to the romfs folder on your sd card. Make a folder called RSDB and place the file in there

20. Boot up the game

Have fun with your new kit but be sure to take a little break if all that code overwhelmed you because the next tutorial will involve a lot of code as well.

# Changing Weapon Functionality / Parameters

This might be the most anticipated part for you. At the end of this walkthough you will be able to change almost anything about any main, sub, and special weapon.

Right now i will just show you how to modify some very basic parameters. After this tutorial though is where everything gets more specific and i show you literally everything i know

Lets change the range, damage, RNG, and fire rate of the Splattershot Nova

This tutorial will have less pictures and less descriptive text for things we've already done multiple times in previous tutotials.

1. Inside toolbox, lets decompress another file with ZSTD compression. You should know how to decompress and compress with ZSTD by now

2. go to your romfs dump and open the Pack folder. Then select `Params.pack.zs`

This file contains all main, sub, special weapon parameters as well as stage parameters

3.  save it as `Params.pack` to a location you can find easily

4.  open the newly saved `Params.pack` in toolbox

We are going to search for the code name of a weapon we want to modify. If you want to modify its functionality specifically for salmon run or hero mode, add `_Msn` for hero mode or `_Coop` for salmon run to the end of the search.

5.  Hit the search button and search for ShooterQuickLong. To find splattershot nova. however this brings up 2 files

<img width="107" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/6b72cce2-f1b0-4ee2-bf7b-95f0b0ef3a21">

<img width="304" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e33eb047-ff30-4360-8afc-baad4aae8a06">

We always want the one that dosent have "Coop" in the name. Coop means Co-op which means salmon run. any file in Params.pack with Coop in the name only changes specific parts of the weapon in salmon run so we dont care about it.

6. Click the file without Coop in the name to locate it in the file view. Close the search window now

7. double click the highlighted file.

8. switch to text editor and hit "Decompile"

Lets start by giving it 100 damage just for the hell of it.

9. Locate the line that says DamageParam. Should be at line 15

10. ValueMax and ValueMin are the only values we care about 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3f69a8f3-b325-4806-b846-fc88b141207f)

11. 240 and 120 are the damage numbers multiplied by 10. the extra zero is in case a decimal value is needed. so lets set the Max and Min damage to 1000 to make it do 100 damage no matter what.

12. Lets also give nova perfect RNG. To do this, scroll down to the bottom section `WeaponParam`

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/4fd0b12c-24ee-442a-924e-0151b75ae3b9)

13. RNG is under the 2 variables that contain `DegSwerve` Jump_DegSwerve is jump RNG and Stand_DegSwerve is ground RNG. set them both to 0

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3a20c4bc-2cec-49c0-aa3b-9442c2587d87)

14. now on to fire rate. the `RepeatFrame` variable. Set it to 1 to make it fire every frame. i dont know what setting it to 0 will do and im too scared to try

15. Finally, range. scroll up to the line called `MoveParam` (should be line 18) and find the variable called `SpawnSpeed`. this is the range. but because its so small, just adding 1 or 2 will make it shoot across the map. although you can set this as high or as low as you want. Set the highlighted value on this line to a larger number
![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fa70d5a0-4ef8-4cae-8843-8a4df3d4853f)

16. click Compile at the top

17. once you save that file, make sure to save the Params.pack file too

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b00f54ea-b1f0-455c-a2c0-421ab5982f02)

18. compress the saved file with ZSTD. and put your newly created `Params.pack.zs` inside the Pack folder in your SD card romfs directory

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/d0844ef8-1f92-4672-b676-60ac8be23e4b)

29. Boot up the game

Nova is finally a functioning weapon. 

and thats basically everything about splatoon 3 modding. the next sections and sub sections of the tutorial are just to be used as reference points for how to do specific things. think of it as the Splatoon 3 API Documentation.

# Specific Weapon Parameters
This section will have sub sections that all focus on telling you where and how to modify more specific weapon functionality. general functions of a class will not be covered as they are either unimportant or easy to understand yourself.

### Ink Consumption
Down in the `WeaponParam` section for your weapon you will find a variable called `InkConsume` this variable tells the game how much ink to remove from the tank **per shot**.

### Paint Parameters
find a section called `PaintParam` these give you a ton of customization for how much paint the weapon does. Multiplying all the values by 10 gives you some really fun results.

### RNG

### Range

### Damage

### Fire Rate

### Chargers - Homemade Aimbot

### Chargers - Increase Air Charge Speed

### Chargers - Force Scope, Divided Shots, and/or Charge Holding

### Dualies - Roll Count

### Dualies - Shoot while Rolling

### Dualies - End Lag

### Shooters - L-3 and H-3 Shooting (3 Shots)

### Shooters - Squeezer Shooting (Semi-Auto)

### Brellas - Undercover Brella Shooting (Keep Sheild)

### Splatanas - 1-Shot Radius

### Brushes - Rolling Ink Resistance

### Brushes - Roll Speed

### Blasters - Intensify Action Reduce RNG

### Blasters - Explosion Radius

### Splatlings - Recharge while Shooting

### Stringers - Charge Hold

### Stringers - Jump Tilt Angle

### Stringers - Guide Trajectory

### Bloblobber - Blob Parameters

### Object Place Number

# Misc

### Ink Splatter Textures

### The Layout Folder

### Stage Editing
Stage editing is pretty complex but right now, its not even possible with most of the stages. toolbox kinda dosent compile some of the byml files correctly so until thats fixed, dont worry about it

### Replacing Fonts


### Closing Notes


