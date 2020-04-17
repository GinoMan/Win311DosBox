# Windows 3.11 DosBox Container Shell #

## Description: ##

Some games or apps of yore will not install on pure dos, instead, they need to be installed and run on Windows 3.11. In order to do this however, you need to have windows 3.11 installed. It's also inconvenient to have all of your games in a single DosBox instance. So what to do? This is a portable Dosbox container running Windows 3.11 in which you can clone this repo, install your game, change the config to run the game automatically, and then link directly to the DosBox runner. 

## HowTo: ##

1. Clone the respository using Git
2. Copy the installation files into "Installer"
3. Run DosBox and install the game by running the installer off the N drive.
4. Close DosBox and open the configuration in `Data/settings/dosbox.conf`
5. Remove the Installer mount line (prepend with a #)
6. Do the same for the settings line
7. Change the last line that runs Windows 3.11 and replace it with the exe for the game.
8. Test DosBox runs the game satisfactorily and then close DosBox
9. Delete the installer folder.

Now, when this instance of DosBox is run, it will immediately open the game. It can then be installed wherever you wish and added to whichever game launcher you wish to use. 

## Future Updates ##

Eventually the box will already have the settings for full screen and stretching. 