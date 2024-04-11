Repo for Sinden soft mod

**DONT USE THIS MODDED VERSION TO UPDATE YOUR LIGHTGUN FIRMWARE. USE THE OFFICIAL APP !**

Emulators that support my Sinden recoil : 

https://github.com/nixxou/Dolphin

https://github.com/nixxou/pcsx2

https://github.com/nixxou/duckstation


A mamehooker dll to make it work with mamehooker : https://github.com/nixxou/PacDriveSDK

Know bug : Currently if you launch a game with recoil support, you can't hit the stop button on the siden software while the game is running.

You can send command lines :

.\Lightgun.exe -action "start"

.\Lightgun.exe -action "stop"

.\Lightgun.exe -action "mouse-pause"

.\Lightgun.exe -action "mouse-resume"

.\Lightgun.exe -action "load-config test.Config"

.\Lightgun.exe -action "restore-config"


When you launch them, it will not popup a new Lightgun app, but send commands to the existing one.

You can also add offsets to a profile with command like : -action "load-config Dolphin.Config:10,20,30,40"

that will set X Offset to 10, X Ratio to 20, Y Offset to 30 and Y Ratio to 40.

To make a profile, just make a copy of the Lightgun.exe.Config after you made all the change in it that you want and rename it. Not sure what happen if you try to save config change once a profile is loaded, so don't do that.

There is an AHK textbox that is part of the config. It's preconfigured to bind to the Lightgun joystick, so you can use function like GUNA_BTN1(value){} to do something when the joystick button 1 of gun A is pressed. (GUNB_BTN16 function will trigger on Gun B, buton 16)
Honestly, i don't use the ahk system currently, but i was too lazy to remove it so i leave it here. Take it as an experimental feature, i made it so if there is only empty lines or comments, it doesn't run ahk at all.


