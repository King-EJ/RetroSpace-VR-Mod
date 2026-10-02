# RetroSpace-VR-Mod
VR Mod for RetroSpace

RETROSPACE VR  -  VR mod for "RetroSpace" (Unity 6000.3, IL2CPP, URP)
=====================================================================

Version 0.1.16 (test build on Quest 3 Virtual Desktop).

WHAT IT DOES
------------
* Stereo VR through OpenXR (SteamVR, Meta/Oculus, Virtual Desktop, WMR...).
* You are the player: the game looks where you look, the left stick walks where you look,
  the right stick turns (snap turn by default).
* The weapon / tool in hand goes to your right hand and fires where you point it (red laser).
  The flashlight beam comes from your left hand.
* The VR controllers act as a gamepad for the game's own controls and menus.
* Doors, buttons and pick-ups are used with your right hand: point at them (with a weapon: the laser)
  and press A. The use prompt (button icon + name) floats above the right controller.
* Health, stamina, the minimap, the flashlight / noise meter, the current objective and what you just picked up
  float above your left controller; the ammo count floats at the right side of your weapon.
* Menus and the inventory are on a screen floating in front of you. Camera shake is off.

INSTALL
-------
1. Copy the zip into the game folder.
2. Start SteamVR (or your OpenXR runtime), then start the game.

CONTROLS
--------
Left stick ......... walk

Right stick left/right .. turn

Right stick up ..... Y (jump)  

Right stick down ........ d-pad up (medkit)

Right trigger ...... fire (RT)  

Left trigger ............ aim (LT)

Right grip ......... RB         

Left grip ............... LB

A .................. A (use)     

Left stick click + A .... d-pad left (PDA)

B .................. X (reload)

Y (tap) ............ d-pad right (flashlight) 

Hold Y .................. laser setup

X (tap) ............ B      

Hold X .................. d-pad down (inventory)

X + Y together ..... pause (Start)

Both stick clicks ....... re-centre

In menus the right stick is the d-pad.

Everything is in BepInEx\config\retrospace.vr.cfg ([Controls] = gamepad buttons, [KeyControls] = keys).

MENUS:                  point your right hand at the screen (blue laser) and pull the trigger.

IN-GAME SETTINGS MENU:  hold Y + left stick click for 1.7 s.

LASER / BULLET POINT:   hold Y for 1.2 s (weapon in hand):
                          left grip (hold) ... grab the yellow start point and put it on the barrel tip
                          right stick ........ steer the laser end (left/right, up/down)
                          right grip (hold) .. the laser stays where it points while you turn the gun
                          B = reset, A = save, hold Y again = cancel
                          
WEAPON PLACEMENT:       hold both stick clicks for 2 s (left grip = grab & move, right stick = size, A = save).

HAND ADJUST:           Hold Y + right stick click for 1.5 s.

MINIMAP POSITION:       
[UI] MapOffset = "x,y,z" from the left controller (x = right, negative = left; y = up; z = forward),
                      
MapScale = size (also in the in-game settings menu), MapOwnSpot = false puts it back in the stack.
                        
LEFT-HAND HUD:          
in-game settings menu -> "HUD on left hand" / "Left-hand HUD size".

USING THINGS:           
[Weapons] InteractAim = Hand (point with the right hand) or Head (look at it).

[UI] UsePromptOnHand / UsePromptScale / UsePromptOffset = the prompt above the controller.

CREDITS & LICENCES
------------------
[RetroSpace](<https://store.steampowered.com/app/2067820/RetroSpace/>) belongs to its developers The Wild Gentlemen. This is a free, fan-made, non-commercial mod.
OpenXR.dll (native OpenXR bridge) by Astien (c) 2025 - free, non-commercial redistribution, see BepInEx\plugins\TTVR\LICENSES.

