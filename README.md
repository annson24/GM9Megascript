# GM9Megascript
An all-in-one solution to your GodMode9 scripting needs!

# How to use:

__For normal gm9 usage:__

1. Download the `GM9Megascript.gm9`
2. Move or copy it to `SDMC\gm9\scripts`
3. Run godmode9 on your 3ds and press the home button.
4. Select `scripts`, and select the `GM9Megascript`.

__For use with PCLess b9s install:__

1. Download the `in-files.7z`
2. Open it and extract the `gm9` folder to the root of SD card.
3. Run godmode9 in any possible way you can and execute the `GM9Megascript`.
Or
Download and run the `GM9Megascript-standalone.firm` in any possible way you can.
4. Choose `Hax Options` > `Install Boot9strap` > `PC-Less Boot9strap`.

# What is PC-Less Boot9strap?

__Here's a long explanation on what it does.__

1. First, it checks the system if `sector0x96` is genuine (usually the check will fail if a9lh is installed in the system).

If the check fails, the script will prompt the user if they want to attempt to fix it. Fixing it, the user should have the `secret_sector.bin` file inside `SDMC/gm9/in/boot9strap` folder.

2. Once confirmed that `sector0x96` is genuine, it'll then check if the required files are present in the `SDMC/gm9/in` folder.

_Here's the branches of the folder that it checks:_

SDMC
* gm9
* * in
* * * boot9strap
* * * Luma3DS
* * * sdcompiled

3. If everything is in check, it'll then backup your boot9.bin and boot11.bin.

4. The script will now install boot9strap.

5. after boot9strap installation, it'll set up Luma3DS to your CTRNAND.

6. Now there is a folder named `sdcompiled`, inside this are all the necessary files we need to have on our sd card after we install boot9strap. Think of this as the finalization proccess on plailect's guide. But since this is a 'PC-Less' installation, this is done purely on the 3ds.

7. The script will copy all the files from `sdcompiled` folder to the RAM of the 3DS, then it'll prompt the user to swap the sd card to whichever sd card the user wants to use. Once sd cards are swapped, the script will then move the files from the RAM to the newly inserted sdcard.

8. After all that, you're done but you'll be given the option to inject FBI to H&S or not before finishing.

__tl;dr__

* The script installs boot9strap
* The script sets up the SD Card and ctrnand for CFW use
* The script injects FBI to H&S (optional)

# Credits:
* mvmiranda - learned the basics from him, he was my mentor.
* d0k3 - basically the god of godmode9
* 8bitwonder - got most of the script from his megathread
* emillois - helping me test and provide info for Old 3/2ds model
* TurdPooCharger - he's the one who figured out how to inject apps to system apps. Inject FBI to H&S is all him.
* Plailect
* AnalogMan
* windows_server_2003
* SvenDaHacker64
* MyLegGuy
* Some1CP
* figgyc
* ihaveamac
