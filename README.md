# OBS-Input-Overlay-for-Dance-Pads
A simple html (java script) overlay for OBS to display Dance Pad inputs (any gamepad abxy inputs), supports L-TEK Pads and others

## Instructions

**1)** Add a new **Browser** source<br>
**2)** Name it whatever you want and click **OK**<br>
**3)** In the **URL** box, enter the file path to where you put **index.html**, **texture.png** must also be there<br>
Also enter the **Width** and **Height**, here it's **260** for both<br>
Click **OK** to update what's shown

![StepsToDo](https://imgur.com/ODiiegc.png)<br>

The grey text will disappear after it detect your pad, reconnect pad if not detected or see instructions to add a 2nd Pad

## If you prefer to not download any files

You can put in https://lninjaplayer.github.io/OBS-Input-Overlay-for-Dance-Pads/ in the **URL** box.

## To add a 2nd Pad

The 1st Pad should have the id 0 if it's the only "gamepad" connected, to have the overlay of another Pad,<br>
Repeat the steps above then in the URL box, add **?pad=1** or increment the number for more Pads at the end just after .html

![For2ndPad](https://imgur.com/JyN1KAn.png)<br>
(You can also put **?pad=0** to indicate the 1st Pad)

## If you prefer to not download any files
Same instructions: https://lninjaplayer.github.io/OBS-Input-Overlay-for-Dance-Pads/?pad=1

## Note

Some presets from [input-overlay](https://github.com/univrsal/input-overlay) might work.<br>
To do so, from the preset's .json, copy everything into **const preset** at line 50 of **index.html** (in-between = and ; )<br>
Then replace **texture.png** with the corresponding texture image PNG from the preset<br>
(modify **atlas.src** at the bottom of **index.html** if you want to change the name).

![Imgur](https://imgur.com/6EVzGZy.png)<br>
(You might want to modify 'const TEXTURE_SPACE' depending on the preset)
