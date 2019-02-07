# NVIDIA_P106
NVIDIA P106 GPUs PLAY GAME
(Tested on Gigabyte 6GB version)
----------------------------------------
open administrative command line
bcdedit /set {current} testsigning on
bcdedit /set {current} nointegritychecks on
reboot

after you are done you can turn off testsigning so steam games(anti-cheat detection) will work again.
bcdedit /set {current} testsigning off

use DDU to uninstall (safe mode unnecessary) 
https://www.wagnardsoft.com/
----------------------------------------
METHOD
----------------------------------------
Modify the'nv_dispi.inf'
----------------------------------------
Open it with Notepad++
----------------------------------------
find all lines with 1C07 and change all Section### to match 1C06 Section###'s
----------------------------------------
i also like to change the following line so that device manager will say that it is a gaming card.
from 
NVIDIA_DEV.1C07 = "NVIDIA P106-100"\
to\
NVIDIA_DEV.1C07 = "NVIDIA GeForce GTX 1060 6G"
-----------------------------------------
Save it
-----------------------------------------
