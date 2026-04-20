# Grahana
Vertical per-app volume control for Linux Cinnamon
<img width="360" height="216" alt="Image" src="https://github.com/user-attachments/assets/e2ed924a-87a4-4e55-837a-51881fffbea2" />
-Displays active audio sources in a vertical format with sliders and media titles from individual browser tabs.

Demo- https://youtu.be/-5W3nlSEZ7g
## Requirements

-Cinnamon Desktop environment
-PipeWire (for media information)

## Installation

1. Download moonstone and sunstone and place them in ~/.local/bin

   - Make them executable (open up a terminal, paste in command and hit enter)
```
chmod +x ~/.local/bin/moonstone ~/.local/bin/sunstone
```
3. Download the grahana@hisovereign folder and place it in ~/.local/share/cinnamon/applets

   -download the metadata.json and the applet.js then create a folder named grahana@hisovereign and place it in ~/.local/share/cinnamon/applets (place the files in folder you made)

4. Restart cinnamon (alt + F2 then type r and hit enter) or restart pc

5. Open applet menu (right-click on panel, click applets) and add the grahana applet from manage tab.

## How to use

-click on grahana applet icon and active sound sources will come up
-sliders change volume 
-click an app icon to mute/unmute sound

## Known behavior

Muting sound from browser will make it an inactive sound source and it will disappear form the list. Unmuting brings it back however this breaks current media information and it will show generic browser name. To fix reload page.

Some browsers currently not supported for media information.

older version of applet used polling which caused noticable micro-stutters in games. New version now only updates on icon click from panel
