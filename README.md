# OBS-Input-Overlay-for-Dance-Pads
A simple html (java script) overlay for OBS to display Dance Pad inputs (any gamepad abxy inputs), supports L-TEK Pads and others

## Instructions

**1)** Add a new **Browser** source<br>
**2)** Name it whatever you want and click **OK**<br>
**3)** In the **URL** box, enter the path to where you put **renderer.html**, **texture.png** must also be there<br>
Also enter the **Width** and **Height**, here it's **260** for both

![StepsToDo](https://imgur.com/ODiiegc.png)<br>

The grey text will disappear after it dectect your pad, reconnect pad if not detected or see instructions under:

## To add a 2nd Pad

The 1st Pad should have the id 0 if it's the only "gamepad" connected, to have the overlay of another Pad,<br>
Repeate the steps above then in the url box, add **?pad=1** or increment the number for more Pads at the end just after .html

![For2ndPad](https://imgur.com/JyN1KAn.png)<br>
(You can also put **?pad=0** to indicate the 1st Pad)

## Note

Some presets from [input-overlay](https://github.com/univrsal/input-overlay) might work.<br>
To do so, from the preset's .json, copy everthing into **const preset** at line 50 of **renderer.html** (inbetween = and ; )<br>
Then replace **texture.png** with the corresponding texture image png from the preset<br>
(modify **atlas.src** at the bottom of **renderer.html** if you want to change the name).

![Imgur](https://imgur.com/6EVzGZy.png)<br>
(You might want to modify 'const TEXTURE_SPACE' depending on the preset)
