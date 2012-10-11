sc-character-import
===================

Character import for use with ShadowCraft scripts.

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

* working python environment (see Setup below)
* ShadowCraft-Engine installed (I used https://github.com/dazer/ShadowCraft-Engine)
* wowapi installed (https://github.com/Dorwido/wowapi)

Setup (Windows):
================

* download and install python from http://www.python.org/download/, I am using python 2.7.3
* download and install setuptools from http://pypi.python.org/pypi/setuptools#downloads, I am using setuptools-0.6c11.win32-py2.7.exe
* add the python path from step 1 to system path (My Computer -> properties -> advanced -> environmental variables -> system variables -> path)
* clone ShadowCraft-Engine (you can download zip from github, or use github client)
* clone wowapi
* clone this repository (sc-character-import)
* Run -> cmd
* go to ShadowCraft-Engine repository (for me it's: cd c:\Users\MyName\Documents\GitHub\ShadowCraft-Engine)
* type python setup.py install --user
* go to wowapi repository
* type python setup.py install --user
* go to sc-character-import repository
* type python mop_assassination.py

If everything worked fine, you should see some EP values and DPS figures. To
get personalized results, you need to edit mop_*.py scripts.

Known issues:
=============

* Stats (attack power in particular) may be imported wrong 
  (see http://elitistjerks.com/f78/t129910-spreadsheets_deep_space_nine/p6/#post2205133)
* It will most likely crash if you try running it on a character
  profile with some gear pieces not equipped
* Weapon type recognition needs work, for now it's 1.8 -> dagger, 1.8+ -> axe
* Professions are not recognized yet

