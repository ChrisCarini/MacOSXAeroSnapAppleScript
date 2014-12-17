# Mac OSX AeroSnap AppleScript

**Mac OSX AeroSnap AppleScript** is a quick fix for getting basic AeroSnap functionality into *OSX*.

## Usage

Either the "***Manual Service Creation***" section or the "***Service Installation***" section need to be followed; not both.

#### Manual Service Creation
1. Open Automator, [Cmd] + [N] -> Service
2. Set the following "Service received **no input** in **anny application**" at the top.
3. On the left actions, scroll down and double click "*Run Shell Script*"
4. Chose "*/bin/bash*" for the Shell, enter the command: *osascript <path_to_script>/WindowsResize.script left*
5. Save the file as something descriptive, such as "***Send Window to Left***"
6. Repeat steps 1-5 for Left, Right and Full (replace 'left' in the shell script line and file description with 'right' & 'full' for a total of 3 services) 

#### Service Installation
1. Open Finder
2. **[Cmd]** + **[Shift]** + **[G]**
3. Type "*~/Library/Services*", hit [Enter]
4. Drag the files **from** the *GitHub Repos Services* folder **to** the *Services folder on your computer*

#### Adding Keyboard Shortcuts to Service
1. Open *System Preferences* -> *Keyboard* -> *Shortcuts* -> *Services* -> *General*, you should see the names of the services you created in the above section.
2. Select the appropiate service and assign the shotcut you wish to use; I assigned **[left]**, **[up]** and **[right]** to **"Window Left"**, **"Full Screen"** and **"Window Right"** respectivly.

#### Removal
1. Open Finder
2. **[Cmd]** + **[Shift]** + **[G]**
3. Type "*~/Library/Services*", hit [Enter]
4. Drag the created services to the Trash