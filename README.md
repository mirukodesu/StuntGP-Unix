# StuntGP-Unix
Running StuntGP on Linux distros using Proton and MacOS Arm & Intel and current limitations with these methods.

# Special Thanks to:
The community on the [Trickstart](https://discord.gg/ykzAWnA) Discord Server

>[!WARNING]
>This was tested on linux **Debian 13** with KDE and MacBook Air M5 with MacOS 27 Public beta 1.

>[!WARNING]
>The new method for Linux only works for cards with **Vulkan** Support, cards without **Vulkan** support MUST use the [old method](), there are currently no workarounds!



# Prerequisites - Old Method
> [Wine](https://www.winehq.org/)

> [PlayOnLinux](https://www.playonlinux.com/en/)

> [A StuntGP Iso](https://www.myabandonware.com/game/stunt-gp-ddu)

> [StuntKit](https://github.com/stuntkit/StuntKit) and [SkScreen Module](https://github.com/stuntkit/StuntKit_modules/releases/tag/v0.3.0) (Optional): [SkFreeze Module](https://github.com/stuntkit/StuntKit_modules/releases/tag/v0.3.0).

> And most importantly patience (A LOT OF PATIENCE)

# INSTALLATION - Old Method
1) Extract the StuntGP iso to a directory accessible to playonlinux
2) Click Install Program on PlayOnLinux
3) Click Install a program thats not present in the list, it should open a window titled "Manual Installation"
4) Click Next
5) Click "Install program in a new virtual drive", and type a name like "stuntgp", this will be the name of the wine directory and prefix
6) Click Next, in this window we want to check the configure wine option, a new winecfg window will open, we are going to switch the windows version from **Windows 10** to **Windows XP**. after changing close this window and click next.
7) Click 64 bits windows installation
8) Then click explore and select the "Setup.exe" file inside the iso you extracted earlier, do not select the autorun.exe file, it wont install SGP
9) Install Stunt GP normally, relax while the installation finishes =)
10) After the installation finishes add a shortcut to the "StuntGP - Configuration" program
11) Close the playonlinux installation window and open the Configuration program, this is going to generate the GAME.CGF file that we need to set our monitor resolution, apply the configuration and click ok.
12) In playonlinux click the "open directory" button and copy the SKScreen module (and the SKFreeze one if you downloaded it) and the StuntKit loader in the game's root folder.
13) edit GAME.CFG with your preferred text editor: set "DISPLAYRESWIDTH" to the **width** of your resolution (For example: 1920) and set "DISPLAYRESHEIGHT" to the **height** of your resolution (For Example: 1080) and save the file.
14) On PlayOnLinux now click Configure click on the name of the wineprefix you set before (Step 5), and click Create a new shortcut, then select the **StuntKit_D3D.exe** and close the window.
15) And Done!

# OPTIONAL - Old Method:
## Want to add StuntGP in your steam library on linux?
1) Make a .sh script named something like "sgp.sh", write "playonlinux4 --run StuntKit_D3D" then make it executable with **chmod +x /path/to/script.sh/**
2) Add the script to steam as a **non steam game**
3) Make sure to **disable** Steam Play for StuntGP in compatibility options
4) Beutify it with some images from [SteamGrid](https://www.steamgriddb.com/game/38317).
5) Done!
<img src="https://github.com/mirukodesu/StuntGP-Unix/blob/main/image.png">

## Want to fix the StuntGP trick timer?
(It seems like the StuntGP Trick timer is **halfed** when we play on refresh rates higher than 60hz. this affects gameplay and requires to hit the Trick key almost *frame perfect* to do tricks while flying)
### The Steam Method of fixing this bug. (requires the game in the steam library so follow the steps before if you want to do this fix)
1) Open Steam and open the properties tab on your StuntGP shortcut in the Steam library.
2) set these launch options: "gamescope -w "WIDTHOFRESOLUTION" -h "HEIGHTOFRESOLUTION" -r 60 -f -- %command%"
<details><summary>Explanation for step 2:</summary>
*What were doing here is that we are creating a [gamescope](https://github.com/ValveSoftware/gamescope) virtual display and we are setting the maximum refresh rate to 60hz, The game will feel choppy if you were playing on higher refresh rates before, but now you can do tricks. 
set the "WIDTHOFRESOLUTION" as the width of your resolution and "HEIGHTOFRESOLUTION" as the height of your resolution*
</details>
3)Play the game

# Q&A:
## But Linux isn't based off Unix its inspired by the Unix Kernel!!!
> this is just a general name for the repo.
## Why not running it with just WINE?
> i don't know why but wine just refuses to start the StuntGP.exe file
## What about Android devices?
> just use Winlator and the iso :)
## Isn't there a compiled StuntGP linux version?
> No, linux wasn't very popular (and was very limited) at the time StuntGP released, so Team17 never did a linux version for the game
