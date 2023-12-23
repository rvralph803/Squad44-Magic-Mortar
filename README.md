Cappys_mortar_calc_v0.15

================ Overview ================

This project was started as a method for quickly adjusting mortar fire for a mortar within Post Scriptum (rebranded to Squad44). 
Initially I just wanted to import the basic functionality of the Squad mortar calculator into an overlay for PS, but the probject
expanded beyond the scope of this quickly.

The current state of the project is a calculator that is intended to work on all screen sizes between 1920p and 8K. 
It contains both basic and extended functions, and it primarily driven through the windows Optical Character Recognition (OCR)
engine, and AutoHotkey script v1.1.

If you hope to use the calculator you may either download the .ahk version for which the source is completely readable,
however you will need to install Autohotkey v1.1 on your system OR you can utilize the compiled executable. 

Ultimately you will have to use the version that makes you feel most at ease, given that compiled executables may fire off 
anticheat or antivirus programs.

=============== How to use ===============
- Boot up the program
- Spawn in and build your mortar location
- Bring up the main map screen by hitting ENTER on your keyboard. This is the primary resource for all calculations and must be
  visible for the program to extract positional data.
- The blue box at the top of the screen provides some information about the configuration. It will change as you use it.
- Hit PGUP to select your mortar type
- Hit Home to import your mortar position -- you will need to do this any time you change mortar locations. You *must* zoom your map
  out all the way and move your mouse *off of the map* somewhere into another area in the screen before hitting home.
- Hit F4 to create a target solution for your first target
- The program will hold up to six (6) targets in memory at the same time. Once additional targets are marked by hitting F4 the
  old targets will be overwritten in order. Most recent target is always highlighted in a dull red.
- Any target which exceeds the mortar's default range will show an "OUT OF RANGE" indication in its solution box.
- Dispersion around the intended target is controllable by hitting UP or DOWN on the keyboard and will adjust in 50m increments
  This dispersion will be shown as a +- value next to the MIL or ANGLE values in the Target solution. It will only update as new
  targets are placed. This feature allows you to target larger areas, knowing your boundary limits.
- If you would like to clear the current array of targets hit F5
- END will exit the calculator
- The program may give pop-ups from time to time prompting you for more information. Occasionally it cannot interpret the position
  from the screen and you will have to type in the correct Keypad string for your target or mortar (eg A14-9-2 or K8-1-2).
  When these errors occur they will dump some text into a file called output.txt in the same folder as the calculator. If you would like
  to help the project out, feel free to send me your output.txt at rvralph803 at gmail dot com
- If the program cannot ever seem to find your position, and returns an image that doesn't show your position, you will need to help it
  by hitting F1 and drawing a selection box around the location data found below the map.

================ Controls ================

- HOME         - This key sets the position of the mortar based off the current player position
- PGUP / PGDWN - Changes the mortar type
- END          - Close the program
- F1           - Select the text grabbing region for positional changes
- F2           - Manually set target location (deprecated)
- F3           - Manually set Mortar location (deprecated)
- F4           - Set a target
- F5           - Clear all targets
- UP / Down    - Change dispersion by 50m
- Shift + INS  - Reboots the calculator entirely


=========== Future Development ===========

- Modifying how the dispersion adjustments are displayed for easier use
- Line based firing with "next in line" feedback
- CTRL + Click based target setting
- Visual pips on the mortar reticle that show target Mil and Angle
- Chat text scraping to allow teammates to request mortar targets by calling out their keypad.  For example "FOB on A14-7-2" would
  autogenerate a new target based off of the chat to target that fob.
