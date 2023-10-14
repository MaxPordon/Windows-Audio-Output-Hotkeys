# Windows-Audio-Output-Hotkeys
A set of hotkeys that allows easy switching between audio outputs.

When installed, the following hotkeys will be active:
- Win+F1: 🎧Headphones (wireless)
- Win+F2: 🔊Speakers
- Win+F3: 🎧Headphones (wired)

# Dependencies
- [AutoHotKey](https://www.autohotkey.com) v2
- [nircmd](https://www.nirsoft.net/utils/nircmd.html)

# Installation
1. If you haven't already, download AutoHotKey version 2 from [here (exe)](https://www.autohotkey.com/download/ahk-v2.exe) or [here (zip)](https://www.autohotkey.com/download/ahk-v2.zip).
2. Download and install NirCmd from [here (x64)](https://www.nirsoft.net/utils/nircmd-x64.zip) or [here](https://www.nirsoft.net/utils/nircmd.zip). **Copy the path to nircmd.exe.**
3. Download [the .ahk file](https://github.com/MaxPordon/Windows-Audio-Output-Hotkeys/blob/main/AHK_v2_Set_Audio_Output)
4. **Make sure that in the code at line 21 **you change `C:\your\path\to\nircmd.exe` to where you installed nircmd.exe**.
5. Make sure your desired audio devices are called exactly "Headphones" and "Speakers" in the Sound Control Panel. To get there:
- Win + R
- type `control mmsys.cpl sounds`
(or Control Panel -> Hardware and Sound -> Sound)
Then if they are not exactly named "Headphones", "Speakers" and "Monitor": rename your desired headphones and speakers devices by right-clicking them and then clicking 'Properties' Note that you could of course also rename the names for the devices in the code. 
5. In order for this to work also after you restart your PC - which you definitely do! :) - do the following:
- Create shortcut of the .ahk file
- Move the shortcut to Windows' startup folder (to get there: in+R -> type `shell:startup`, Enter)

All done!
