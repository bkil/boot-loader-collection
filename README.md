Archive of sample boot loader binaries from the wild
=

Goal
-

Every model of wireless device should have at least one sample here.
It is a plus to gather all builds of boot loaders for a given model.

Use
-

* brick recovery,
* open source firmware compatibility testing.

Contributing
-

Please send a pull request to add your own sample to the collection.

Use the folder corresponding to the chipset of your CPU.
You can find this at various sites online, such as:

* https://www.wikidevi.com/
* https://www.openwrt.org/
* https://wiki.dd-wrt.com/wiki

To make the filename unique, it should contain:
  
* the exact device model,
* the exact model version (+board revision),
* u-boot build date: strings *|grep U-Boot,
* +the specific region code if printed (EU, HU, INTL, ...),
* +your name,
* +your MAC (or at least a few bytes from the end).

For example, the following could be valid filenames:

* `AR9331/TL-WR740N_v4_2015-07-01T141146_bkil.bin`
* `AR9331/TL-WR740N_v4.32_HU_U-Boot_1.1.4_2015-07-01T141146_bkil_11:22:33:44:55:66.bin`

The bulk of the information lies in the model number and the others are
contained in the file itself, so a shorter form might suffice in most
cases. Although there could exist builds with hard coded flash chip IDs
suited for given board revisions as well, so just to be on the safe
side, please share as much information as possible.

You should add metadata including references, contact, and site of
original publishing to your commit message.

License
-

(C) Copyright 2000 - 2013 Wolfgang Denk, DENX Software Engineering, wd@denx.de.

U-Boot is Free Software.  It is copyrighted by Wolfgang Denk and
many others who contributed code (see the actual source code and the
git commit messages for details).  You can redistribute U-Boot and/or
modify it under the terms of version 2 of the GNU General Public
License as published by the Free Software Foundation.  Most of it can
also be distributed, at your option, under any later version of the
GNU General Public License -- see individual files for exceptions.

For a full list of terms, please check the source code at the
official repository:

* https://git.denx.de/u-boot.git/

Source code for builds customized by the manufacturer can be obtain from
their official website:

* https://www.tp-link.com/us/support/gpl-code-center
* https://kb.netgear.com/2649/NETGEAR-Open-Source-Code-for-Programmers-GPL
* http://tsd.dlink.com.tw/GPL.asp
* http://www.zyxel.com/us/en/form/gpl_oss_form.shtml
* http://www.belkin.com/us/support-article?articleNum=51238

For some more documentation on how to build, see:

* https://openwrt.org/docs/techref/bootloader/uboot
* https://github.com/doozan/uBoot
* https://github.com/pepe2k/u-boot_mod

See also
-

* https://github.com/bkil/calibrated-art-collection
