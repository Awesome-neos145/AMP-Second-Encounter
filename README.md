# awes145's Mission Pack - Second Encounter
A mission pack for the Macintosh version of Wolfenstein 3D.
# Installation
## ****This scenario requires that the *Third Encounter* missions be installed. Take this as your warning.****
There are multiple ways to go about playing and installing this pack. We will start with the Macintosh version first.

If you're using an emulator like Sheepshaver, mount the disk file and then boot up the system. Open the disk titled "awes145's Mission Pack"...

![Mounted AMP disk](https://file.garden/YtxRl-gHkWVkfPs7/images/figure1.png)

...and drag it into the Levels folder where your Wolfenstein 3D installation resides.

![Installation Procedure](https://file.garden/YtxRl-gHkWVkfPs7/images/Screen%20Recording%202025-11-15%20161126.gif)

Then start Wolfenstein 3D and choose the scenario from the list.

![](https://file.garden/YtxRl-gHkWVkfPs7/images/scenario.png)

A copy of the instructions are located in the disk file.
A Stuffit file is also included incase you need to somehow download it to the machine.
QuickTime is needed to display the image on the Scenario Select screen but is not a requirement.
# DOS
<small>*oh you thought this was a mac only thing huh*</small>

To get this to work, you need to get all the levels from the Levels folder to your PC. They must be in either AppleDouble format or Resource format. If you don't want to do that, click [here](https://archive.org/details/macwolfensteinresources).
Next you'll need the source from [FrenkelS/Wolf3D-Mac-for-DOS](https://github.com/FrenkelS/Wolf3D-Mac-for-DOS).

Download the source code and place the Resource-formatted files into /wad/src/main/resources/input/. It should look like this:

![](https://file.garden/YtxRl-gHkWVkfPs7/images/fig2.png)

Next, grab the latest version of [Maven](https://maven.apache.org/download.cgi). Extract that and put it somewhere. Add /mvn/bin/ to PATH (or you can drop the batchfile in a command prompt, either way is fine)
Now run `mvn verify`. It will start compiling all of the Resource files it detects into WAD files for you.

Once that's done, go back to the Wolf3D Mac for DOS page but now download the [prerelease-release](https://github.com/FrenkelS/Wolf3D-Mac-for-DOS/releases/tag/v20250716). Extract that and put the generated WAD files into the folder.

In a DOS emulator, you should run `mw(arch)m(vidmode) file MAPS1.WAD`

...where (arch) is either 286/386 and (vidmode) is y/13. You can rename MAPS1.WAD to anything, as that should be the generated AMP Second Encounter WAD. I also included some laumchers for MacWolf if you want them here.

# Windows
We are using [LateGator/MacWolfSDL](https://github.com/LateGator/MacWolfSDL) here.

Resource format files are [here](https://archive.org/details/macwolfensteinresources).

To make this work, grab the AppleDouble, Resource, or MacBinary files and place them in `C:\Users\<USER>\AppData\Roaming\macwolfsdl\`. The Third Encounter + Second Encounter (also AMP) files should be placed in `/Levels`, while you should just place the `Wolfenstein 3D` executable in the root of the `macwolfsdl` folder.

It should look like this:

![](https://file.garden/YtxRl-gHkWVkfPs7/images/fig3.png) ![](https://file.garden/YtxRl-gHkWVkfPs7/images/fig4.png)

Start MacWolfSDL and choose the AMP scenario from the menu. (you can also choose the scenario by pausing the game and choosing `Load Scenario...`)

![](https://file.garden/YtxRl-gHkWVkfPs7/images/fig5.png)

# Conclusion
That should be all! Let me know if you have questions.

...
# Where the hell are the next 3 Episodes?
They're gonna come later under the name "Die Ballade vom Todesmeister". Please be patient.
# Where can I run this?
You can run this under anything that is decent at emulating MacOS. For example, InfiniteMac or Sheepshaver. Basilisk II should work. Mini vMac will not work because the FPU emulation is very far from complete.
# Where can I even get the Mac version of Wolf3D?
Check Macintosh Repository.
