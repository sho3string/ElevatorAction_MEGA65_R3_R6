Elevator Action - for MEGA65
============================

Elevator Action is a classic arcade video game that originated in 1983 and quickly became a standout title in the golden age of arcade gaming. Developed by Taito, Elevator Action is renowned for its innovative gameplay and unique premise.

In Elevator Action, players take on the role of a secret agent tasked with infiltrating a high-rise building filled with enemy agents. The goal is to retrieve secret documents hidden within the building's various floors while avoiding or eliminating opposition along the way.

The game's primary mechanic revolves around navigating elevators and escalators to move between different floors of the building. Players must strategically time their movements to avoid enemy agents and utilize the elevators to their advantage. Elevator Action's dynamic level design, coupled with its challenging enemy encounters, adds an engaging layer of complexity to the gameplay.

As players progress through the levels, they encounter various obstacles and adversaries, including armed guards, surveillance cameras, and other hazards. Elevator Action's combination of stealth, strategic planning, and action-packed sequences provides a unique gaming experience.

Elevator Action features classic pixel art visuals and an iconic soundtrack that contributes to the overall nostalgic charm of the game. Originally designed for arcade cabinets, Elevator Action has been adapted and preserved through various platforms and emulators, allowing players to enjoy its timeless gameplay.

This core is based on the MiSTer Elevator Action core, leveraging the collaborative efforts of the MiSTer community. The MEGA65 adaptation of the Elevator Action core was accomplished in 2023 by [Developer Name], utilizing the MiSTer2MEGA65 framework and incorporating QNICE-FPGA for FAT32 support and on-screen menu functionality.


[MiSTer](https://github.com/MiSTer-devel/Arcade-TaitoSystemSJ_MiSTer) ElevatorAction core which itself is based on the work of [many others](AUTHORS).

[Muse aka sho3string](https://github.com/sho3string)
ported the core to the MEGA65 in 2024.

The core uses the [MiSTer2MEGA65](https://github.com/sy2002/MiSTer2MEGA65)
framework and [QNICE-FPGA](https://github.com/sy2002/QNICE-FPGA) for
FAT32 support (loading ROMs, mounting disks) and for the
on-screen-menu.

How to install the core
-----------------------

1. **Download ROM**: Download the Elevator Action MAME ROM ZIP file from the internet.
   Search for the Elevator Action bootleg rom ( elevatorb ).

   Ensure that the set you're using has the following files or the conversion will fail.  
   <img width="940" height="597" alt="{64323443-3BAE-4E3A-AAD8-73E0F66903E0}" src="https://github.com/user-attachments/assets/7c4582c5-1615-44c1-8a06-7f35b463a807" />
 
3. **Download the batch or shell script**:
   a. [Link](https://github.com/sho3string/ElevatorActionMEGA65/blob/master/ElevatorAction_rom_installer.bat) ( For Windows  )
   b. [Link](https://github.com/sho3string/ElevatorActionMEGA65/blob/master/ElevatorAction_rom_installer.sh)  ( For Unix/Linux/MacOS )

4. **Run the script**:  
   a) First extract all the files within the zip to any working folder.  
   
   b) Copy the batch or shell script to the same folder and execute it to create the following roms => maincpu.rom, bankedcpu.rom, soundcpu.rom, video.rom, layer.rom and eacfg  
   
   For Windows  
    `ElevatorAction_rom_installer.bat`  
       
   For Unix/Linux/MacOS  
   `./ElevatorAction_rom_installer.sh`

   Example output using the bash script  
   <img width="537" height="328" alt="image" src="https://github.com/user-attachments/assets/7728277f-1f2e-473f-aac4-9c9534d4642b" />

6. **Copy the ROMs to your MEGA65 SD card**: Copy the files with your generated ROMs tothe MEGA65 SD card. You can use either the bottom SD card tray
of the MEGA65 or the tray at the backside of the computer (the latter has precedence over the first).
   '**maincpu.rom, bankedcpu.rom, soundcpu.rom, video.rom, layer.rom and eacfg**' need to be in the folder `arcade/elevator` on the SD card or the game will not run.

   Ensure hat the generated rom files have the correct file sizes  
   <img width="529" height="96" alt="image" src="https://github.com/user-attachments/assets/c0d41fe4-bf1d-444c-8982-0d4b45363c5c" />

8. **Setting up dip switches**

   Enter the Game Setup by pressing the 'HELP' key, set the individual dip switches for that version in the dip section. There are three dipswitch settings.

   See below for description of dip settings to customise your game.
   
   https://www.arcade-museum.com/dipswitch-settings/7700.html

   Once done, press the reset switch on the MEGA65 to load the new settings.


   
    
