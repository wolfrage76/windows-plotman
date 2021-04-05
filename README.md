# `windows plotman`: an attempt to get plotman to work on windows

THIS IS A BETA.  Not ready for production use just yet.  Almost, but not quite there yet.

This is a tool for managing Chia based on Plotman (https://github.com/ericaltendorf/plotman)

This is a work in progress. Please see the original linux version for additional info:

https://github.com/ericaltendorf/plotman

Please contact me at: chia@ifhya.com or Wolfrage on discord in the #chia channel: https://discord.gg/JESmva9R - pop in and say hi!

## Known issues:

- Archiving hasn't been touched
- IO stats does not work on windows
- Resizing terminal messes up the curses display
- Common dir prefix does not work so whole dir path is shown for temps and dest drives
- Various other issues

## Installation

Copy your chia.exe file to chia2.exe and use that for now!  Avoids conflicts with plots running from GUI or commandline.  Will adjust after testing complete.

This program requires `psutil`, `pyfakefs`,`texttable`, `windows-curses`, `pyreadline`, `pyyaml`, and `pypsutil`.

First, Edit manager.py to hardcode your chia.exe location (sorry, manual for now). Second, Edit config.yaml for your settings. Third, provide feedback and help me with this because I am soooo not a python guy. I'm really, really, really not. Fourthly, send me pizza.

Run command in Windows Powershell: `python plotman.py interactive`

![image](https://user-images.githubusercontent.com/75458290/113492313-8c0ad680-94a4-11eb-93da-e93521dddde3.png)
