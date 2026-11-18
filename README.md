# Y1_RockBox_CodecSkin
A Metal Gear Solid inspired skin for Innioanis Y1 on RockBox

This theme takes heavy inspiration from the menu elements of Metal Gear Solid Subsistence for the menus, as well as the codec for the now playing screen.
Nods to the series include static text elements on the .sbs screen taking inspiration from text within the wall textures in VR levels. Likewise the bounding box used for "PLAY" status etc. is based on the "VR-SYSTEM" text found on a few wall panels within the VR levels. 
The battery indicator on the .sbs screen is a nod to the MGS2 style alert/evasion/caution radar phases, while in the Now Playing screen the MGS1 radar was used where I felt there was more space to play with. 
It may not be visible, but there having spent so long looking at the images in game, I noticed there is morse code equivalents for Alert and Evasion in the original images. So of course I updated this as needed. Couldn't not do that after figuring it out! :P 


Various sources were used as a reference to understand the behavior of the RockBox coding engine, so a special shout out goes to those below. All of which can be found in the following repository.[https://github.com/rockbox-y1/themes](url)
  INTERPODS     by Christian Soffke
  bunnyPod      by Monica G.
  SNARTY        by Simon Anden
  BONES         by Chuck Largo
  SNAZx90       by DillMillz

Fonts
  MGS2MenuFont        by Solid Snake's Game Shrine   https://fontmeme.com/fonts/mgs2-menu-font/
  AV07AltRationMGS2   by AV Perth (ConEAP)           https://fontstruct.com/fontstructions/show/2049324/av07-ration-mgs2-1
  MGS2InventoryFont   by @the_blue_toad              https://fontstruct.com/fontstructions/show/2938858

Images
  No assets have been extracted from original game files. All images within the folder ".rockbox/wps/MGcodec" were created by myself in InkScape. 
  I spent most of my time on this project using reference images and my own game screenshots trying to get the images as pixel perfect as I could to achieve the look I wanted given the limitations of the Y1 screen. 
  All reference images and original design are the copywrite of Konami. 

Some alternate text colour options I experimented with that may be of interest should you wish to modify your .sbs or .wps files. 

  MGS2 Menu Style Golden Yellow =                          c1a220
  MGS2 Menu Style Unselected Dark Grey =                   313332
  [ALTERNATIVE] MGS2 Menu Style Unselected Light Grey =    4e504f
  MGS2 Menu Style Selection Grey =                         a6b3ac
  MGS1 Codec Green =                                       26665b
  White =                                                  ffffff

How to use:
  Download the zip file, and extract. Connect your Y1 to your computer and navigate to the ".rockbox" folder. Note this may be hidden. 
  Copy the the ".rockbox" folder from your extracted .zip file and copy it to your Y1 in the same level as the preexisting ".rockbox" folder. Write into the existing folders and disconnect. 


Note on development & known bugs
  This theme was created without the use of any AI chatbots, image generators or coding agents. 
  The documentation on the RockBox wiki and a few preexisting themes, credited above, were helpful if anyone wants to look into doing one of their own. 
  https://www.rockbox.org/wiki/CustomWPS.html 
  
  A number of inconsistencies persist that I will not be working to resolve. Known bugs / quirks are:
    Brackets may become cut off at the top and bottom where Rockbox does not draw above and below a certain glyph height
    The battery meter on the home screen will flicker while changing screens. I know there is a sequencing to the clear screen command that is impacting this but I have not been able to figure this out. 
    Some menu elements have been turned off from the main menu. These can be re-instated by removing the "#" on line 44, and deleting ALL of line 46 & 47 within file "MGcodec.cfg". This was down to my own usage habits on the Y1 and some menu elements may not be consistent with the rest of the theme as these have not been developed. 
    While the colour theme for the main menu looks and works how I want it to, when holding the "return/menu" key on the top of the scroll wheel, the text here is dark as I could not get this to be drawn with its own colour code. 

Future Development
  I will not be making any future updates to the repository. While this was a fun project, I think I have reached the limits of what rockbox and myself can do when considering how I would like to see this evolve. 
  If anyone wants to continue to develop this, I have no problems with this. I would appreciate it is the work here was referenced.
