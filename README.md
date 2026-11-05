# We have a new method + Archiving repository
Me, Claude and Dreiji joined forces to make a ported version of StuntGP for MacOS and Linux, it uses the Vulkan and Metal renderers and runs natively on Arm and x86/
For now this repository is no longer manteined and its getting archived./
The new repository is located at: [StuntGP-CrossPlatform](https://github.com/mirukodesu/StuntGP-CrossPlatform)/

# StuntGP-Unix
Running StuntGP on Linux distros using Proton and MacOS Arm & Intel and current limitations with these methods.

>[!NOTE]
>This was tested on linux **Debian 13** with KDE and MacBook Air M5 with MacOS 27 Public beta 1.

>[!NOTE]
>The old methods have been moved to a diffrent file to minimize clutter, [click here](Old-Methods.md) to access the file.

>[!WARNING]
>The new method for Linux only works for cards with **Vulkan** Support, cards without **Vulkan** support MUST use the [old method](Old-Methods.md), there are currently no workarounds!

# Special Thanks to:
The community on the [Trickstart](https://discord.gg/ykzAWnA) Discord Server

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
> There is now :)
