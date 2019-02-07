# NVIDIA_P106
NVIDIA P106 GPUs PLAY GAME
(Tested on Gigabyte 6GB version)

open administrative command line

<b>bcdedit /set {current} testsigning on</b>

<b>bcdedit /set {current} nointegritychecks on</b>

reboot

after you are done you can turn off testsigning so steam games(anti-cheat detection) will work again.

# bcdedit /set {current} testsigning off

use DDU to uninstall (safe mode unnecessary)

# https://www.wagnardsoft.com/

METHOD currently for driver version 416.34: https://lmg.gg/8KV93
----------------------------------------
Extract the .exe using winrar or 7zip.
Modify the'416.34-desktop-win10-64bit-international-whql/Display.Driver/nv_dispi.inf'

Open it with Notepad++

find all lines with <b>1C07</b> and change all <b>Section###</b> to match <b>1C06 Section###'s</b>

I also like to change the following line so that device manager will say that it is a gaming card.
----------------------------------------
From:

<b>NVIDIA_DEV.1C07 = "NVIDIA P106-100"</b>

To:

<b>NVIDIA_DEV.1C07 = "NVIDIA GeForce GTX 1060 6G"</b>

Save it, install from '416.34-desktop-win10-64bit-international-whql/setup.exe'
-----------------------------------------
