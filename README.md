sc-character-import
===================

Character import for use ShadowCraft scripts.

This is quick and dirty implementation of character import from
battle.net profiles.

Included example shadowcraft scripts are taken from ShadowCraft
(https://github.com/dazer/ShadowCraft-Engine). I did not write them.
I only edited them to use this character import instead of fixed
values. To run them for your character you need to edit them and
replace region, realm and character name with your own.

For guide on editing ShadowCraft scripts, look here: 

https://github.com/dazer/ShadowCraft-Engine/wiki/Customizing-the-Spec-Scripts


Requirements:
=============

* working python environment
* ShadowCraft-Engine installed (I used https://github.com/dazer/ShadowCraft-Engine)
* wowapi installed (https://github.com/Dorwido/wowapi)


Known issues:
=============

* Stats (attack power in particular) may be imported wrong 
  (see http://elitistjerks.com/f78/t129910-spreadsheets_deep_space_nine/p6/#post2205133)
* Glyphs are not imported yet
* It will most likely crash if you try running it on a character
  profile with some gear pieces not equipped
