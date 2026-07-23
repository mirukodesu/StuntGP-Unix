

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
