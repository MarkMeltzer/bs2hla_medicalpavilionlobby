![What an amazing logo, right?](/logo.png)

# Description
This little program lets you decrypt a Bioshock addon zip using the original Bioshock game files. **Neither this nor the encrypted addon zip contain any of the copyrighted original Bioshock assets**, you will need to provide these yourself by following the steps below. 

The addon zip is encrypted by doing a bitwise XOR on the zip and a combination of Bioshock game files. Decrypting is done by doing another bitwise XOR on the encrypted zip and the same combination of Bioshock game files.

# Requirements
- BS2HLA.exe
- An installation of Bioshock (the original, not the remaster)
- An installation of Half Life: Alyx
- The encrypted addon zip
    - You can get this here: https://alyxmods.com/mappage?m=56-Bioshock%20Medical%20Pavilion%20Lobby

# How to use
1. Run the BS2HLA.exe (problems? See notes below)
2. Provide the path to your Bioshock installation. For example: *C:\Program Files (x86)\Steam\steamapps\common\Bioshock*.
3. Provide the path to the encrypted zip. For example: *C:\Program Files (x86)\Steam\steamapps\common\Half-Life Alyx\medical_pavilion_lobby.zip*.
4. Provide the path to your Half Life: Alyx installation. For example: *C:\Program Files (x86)\Steam\steamapps\common\Half-Life Alyx*.
5. Hit decrypt and let er ripp.
6. Select the map from "Local Addons" in game.
7. Enjoy!

# Notes:
- The zip does not contain any original Bioshock assets. You WILL need to provide these assets yourself or the data is useless.
- It can take a couple of seconds for the program to start up, please be patient :)
- Windows is not a fan of unknown executables so will throw up a smartscreen window. Just press "More info" and "Run anyway".
- It's also possible that your anti-virus might see the program as a virus. You can add an exception for BS2HLA.exe or if you don't trust it use the instructions below to run the source python script directly.
- The python script is frozen to an executable using pyinstaller 3.4 (newer versions will not work as well and make the executable cause a bunch of anti-virus triggers).

# Run the python script
Note: the python script does exactly the same thing as the executable. Only use these steps if you have problems with the executable or you don't trust the executable.
1. Have python 3.6 or higher installed.
2. Make sure python is added to the PATH enviroment variable.
3. Download the python script from this page (top right -> green "code" button -> Download zip)
4. Open a command prompt (Ctrl+R -> "cmd" -> Enter)
5. Use the following command: *cd* [path of the folder which contains the .py file]
6. Use the following command: *python bs2hla.py*
7. Follow steps from how to use from step 2 onwards.

# Thanks
- Thanks to [nicolas-siplis](https://github.com/nicolas-siplis) for testing and contributing to the code.
- Thanks in general to the [Half-Life: Alyx Modding Hub discord server](https://discord.gg/4djZFKJ) for help with HLA modding.
