# Legie-Fullscreen-Fix
This repo contains fixed .exe file for the game called "Legie"

=================================
I went through a lot of assembly code, which I do not fully understand just to get it running.
With a bit of help from AI, which I don't really like to use, I was able to change some variables inside this file so the game now runs at 1920x1080 resolution.

When I started, I just thought it would be as easy as just finding some argument in a function that creates windows that I could change to make windows re-sizable
but unfortunately, it just wasn't there, so I tried to change width and height parameters somewhere inside code, and it kinda helped, but the real problem is that
even if the game is being displayed in 1920x1080 it still works in 1024x768, but why ? well, because.
Real breakthrough came once I read some comment on steam, that .ini file has a "scale factor" as setting which I obviously missed while checking this file before
but as it turned out, it wasn't a factor or multiplier, this "scale=2" parameter is kind of a preset of game resolution, so the only workaround I found is to simply
use different resolution when preset is set as 2.
=================================

HOW TO MAKE IT WORKING:
Simply download and paste it inside your game folder, but change legie_fixed to legie.exe renaming original file to something other beforehand. Enjoy.
I'm not sure if it's 100% working, and it has some clipping problems but it's still better than nothing.
