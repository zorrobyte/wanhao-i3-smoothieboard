# wanhao-i3-smoothieboard

This is my WIP working config for the Wanhao i3 v2 with Smoothieboard X5, E3D Titan, E3D V6 hotend and BLTouch.

Please don't slap this config on your Smoothieboard and expect it to work. This can lead to printer damage or personal injury.

Read through the repo's issues, add new ones as needed and browse through the commit log. I try to keep good comments when possible.

Here is my start script for 3 point leveling:
G28 #home
G1 Z15 #move probe up 15mm
M280 S3.0 #deploy probe
G32 #level bed
M280 S7.0 #retract probe
G28 #home
