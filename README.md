# RenmeterFoldMod
Rainmeter Skin based un UnFold by  DevilRev
Original skin by DevilRev: https://www.deviantart.com/devilrev/art/unFold-A-Launcher-618503449


This is a modified version of the Unfold skin for rainmeter. 

![Alt text](Screenshots/ScreenMain.png?raw=true "screenshot")


What is different.
Essentially this version aims to make customisation of your launchers much simpler.

The first Big difference is that I implemented launcher for the right side of the scree aswell
For each launcher ther are two files "Discord_L","Discord_R" for left and right version of the launchers.

Next I implemented a variables architecture. Meaning that you can change certain part of your launchers appearance with within just one file.

In the orriginal version each launcher was simply one image file and if you wanted to change the look of it you would have to do it manually in a foto editing software more importantly you would have to do it for every single icon wich can be a huge time if you have a lot of them.

In my version there are still icons but just the icon itself without its text and box.
The Text and background shape is directly drawn by rainmeter.

Drawbacks.
In theory this gives you less visual controll overall since with this current setup you can only make the background shapes square or varous levels of round, so you cant make crazy grafics or other special thing that a image software would allow you too. However due to the fact that you can change quite some parameters for all your launchers instantly I would argue that this is a much better solution overall.

Theoretically this also means more cpu overhead since we need to do more draw call I'm not super into how rainmeter handels it's draw commands and if it can render them efficiantly. However since my image files for the icons are smaller in my version there should be less memory usage.


One thing to note when you create custom icons is that I recomend that you keep them grayscale and Pure White since then you can use the color tint setting so change all of the icons color to whatever you want anytime.
Only if you want to have differently collored icon should you store have colored icon images.
In that case you have to set the color tint setting to 255,255,255,255

Here is the full list of currently supported settings.


[Variables]

;==== background shape variables
sRound =16  //  Amount of roundness to the Background Shape 0 = Rectangle, 25 = Circle  100 = max Elipse
sColor = 255,255,255,30 // color of the background shape

;==== Icon varialbles
iColorTint = 0,0,0,255  ; Color Tint for icons.  If incon img is not white but uses colors then set this to White (255,255,255,255)


;==== Text Variables
tColor =255,255,255,200 // text color
tFont = Roboto Regular // wich font to use ->Fonts are stored in @Recoursces folder
tSize =18 // Font Size
tYValue = 8 // vertical offset for text. ->if you change font size the text wont be centered vertically anymore, use this to recenter them

;==== Animation Variables
aUnfoldSpeed=10  // speed at which the launchers unfold (open)
aDefoldSpeed=5	// speed at which they close

;==== Disk Drives Variables
; Disk Free space Bar Colors
// the included disc launchers have a custom progress bar for how much space of their capacity they have used. 
dColorFree =44,51,126,80  
dColorUsed =30,172,231,220
dBarHeight = 5
dBarOffsetY = 40







