# Wolfenstein: Enemy Territory scripts
## Description
This is mainly meant as a backup for my scripts and configuration files, but feel free to use any part of it yourself, build on it, or just get some inspiration from it. Maybe this is helpful to anyone else :)
## Files
I will shortly list what each file is. If you want to know how to use one of the script files, you can open it to see its interface documented at the top. You can also look at `scripts.bbk.cfg` for an example of usage.
### autoexec.cfg
This file automatically gets executed once when you launch the game. It calls the general configuration file `bbk.cfg`, as well as the scripts setup file `scripts.bbk.cfg`
### autoexec_\<mapname\>.cfg
These files are executed automatically when the map with the given name is loaded. They are used to set map-specific names for spawn points when using `spawn.bbk.cfg`, as well as set the correct spawn timer interval automatically for `timer.bbk.cfg` and `stshare.bbk.cfg`
### autoexec_default.cfg
This file is called when there is no autoexec for the specific map available, and resets the spawn point names and spawn timer interval to their default values (cleaning up from previous maps)
### autoexec_(allies|axis|spectator).cfg
These files are executed automatically when joining the given team. They are used in conjunction with the `autoexec_<mapname>.cfg` files to set the spawn point names and spawn timer for a map.
### bbk.cfg
This is my personal game settings file. You probably want to replace this with your own preferred settings.
### class.bbk.cfg
A class picker script to set up binds to switch classes and teams
### dynashare.bbk.cfg
A script to quickly share with your teammates when a dynamite is going to exploded, based on the plant time.
### kputil.bbk.cfg
A small utility script to make it much simpler to bind keypad keys despite other scripts using the keypad for input
### scripts.bbk.cfg
This file loads and sets up binds for all the scripts you want to use. You can use this as an example on how to set up the specific scripts you might want to use.
### spawn.bbk.cfg
A script to set up binds to switch spawn points quickly. Using the map and team autoexec files mentiond above will give a map-specific name to the different spawn points instead of just a number.
### stshare.bbk.cfg
A script to quickly share the enemies spawn times with your allies.
### stwrapper.bbk.cfg
If you want to use both `timer.bbk.cfg` and `stshare.bbk.cfg`, you can use this wrapper the keep their interval the same at all times.
### timer.bbk.cfg
A script to step through different spawn time intervals and sync a timer to the enemy's spawn time.
