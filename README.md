# GM9Megascript
An all-in-one script consisting of almost all available gm9 scripts I can find.

How to use:

For normal gm9 usage:

1. Download the "AIO Megascript.gm9"
2. Move or copy it to sdmc\gm9\scripts
3. Run godmode9 on your 3ds and press the home button.
4. Select "scripts," and select the AIO Megascript.

For use with PCLess b9s install:

1. Download the "AIO Megascript.gm9"
2. Move or copy it to sdmc\gm9\scripts
3. Download the "PCLessB9SPack.7z" and open it.
4. Inside the archive, find and extract the "annson24" folder to the root of your sdmc.
5. Use NTRBoot to run godmode9.
6. Press the home button, select "scripts," and select AIO Megascript.
7. Choose "InstallBoot9Strap" option and select "PCLessInstall"


What is PC-Less Boot9strap?

Here's a brief explanation on what it does.

1. First, it checks the system if sector0x96 is genuine (usually the check will fail if a9lh is installed in the system).

If the check fails, the script will prompt the user if they want to attempt to fix it. Fixing it, the user should have the secret_sector.bin file inside sdmc/annson24/boot9strap folder.

2. Once confirmed that sector0x96 is genuine, it'll then check if the required files are present in the sdmc/annson24 folder.

Here's the branches of the folder that it checks.

SDMC
 annson24
  boot9strap
   boot9strap.firm
   boot9strap.firm.sha
  Luma3DS
  sdcompiled

3. If everything is in check, it'll then backup your boot9.bin and boot11.bin.

4. After that, the user will be ask if they want FBI to be injected to H&S; If chosen 'yes,' the script will automatically inject FBI to H&S; if chosen 'no,' the script will continue without FBI injection.

5. The script will now install boot9strap.

6. Now that boot9strap is installed, it'll set up Luma3DS to your CTRNAND.

7. now within the annson24 folder, there is another folder named 'sdcompiled' inside this are all the necessary files we need to have on our sd card after we install boot9strap. Think of this as the finalization proccess on plailect's guide. But since this is a 'PCless' installation, this is done purely on the 3ds.

7.1 the script will copy all the files from 'sdcompiled' folder to the RAM of the 3DS, then it'll prompt the user to swap the sd card to whichever sd card the user wants to use. Once sd cards are swapped, the script will then move the files from the RAM to the newly inserted sdcard.
