# GM9Megascript
An all-in-one script consisting of almost all available gm9 scripts I can find.

How to use:

For normal gm9 usage:

1. Download the "AIO Megascript.gm9"
2. Move or copy it to sdmc\gm9\scripts
3. Run godmode9 on your 3ds and press the home button.
4. Select "scripts," and select the AIO Megascript.

For use with PCLess b9s install:

1. Download the "AIOMegascript-Standalone.7z"
2. Open it and extract boot.firm and the "gm9" folder to the root of SD card.
3. Use NTRBoot to run the AIOMegascript-Standalone.
4. Choose "Hax Options > Install Boot9strap > PC-Less Boot9strap."


What is PC-Less Boot9strap?

Here's a brief explanation on what it does.

1. First, it checks the system if sector0x96 is genuine (usually the check will fail if a9lh is installed in the system).

If the check fails, the script will prompt the user if they want to attempt to fix it. Fixing it, the user should have the secret_sector.bin file inside sdmc/gm9/in/boot9strap folder.

2. Once confirmed that sector0x96 is genuine, it'll then check if the required files are present in the sdmc/gm9/in folder.

Here's the branches of the folder that it checks.

SDMC
* gm9
* * in
* * * boot9strap
* * * Luma3DS
* * * sdcompiled

3. If everything is in check, it'll then backup your boot9.bin and boot11.bin.

4. After that, the user will be ask if they want FBI to be injected to H&S; If chosen 'yes,' the script will automatically inject FBI to H&S; if chosen 'no,' the script will continue without FBI injection.

5. The script will now install boot9strap.

6. Now that boot9strap is installed, it'll set up Luma3DS to your CTRNAND.

7. Now  there is a folder named 'sdcompiled,' inside this are all the necessary files we need to have on our sd card after we install boot9strap. Think of this as the finalization proccess on plailect's guide. But since this is a 'PC-Less' installation, this is done purely on the 3ds.

8. the script will copy all the files from 'sdcompiled' folder to the RAM of the 3DS, then it'll prompt the user to swap the sd card to whichever sd card the user wants to use. Once sd cards are swapped, the script will then move the files from the RAM to the newly inserted sdcard.


Credits:
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
