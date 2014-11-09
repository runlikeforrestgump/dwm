Patches for dwm (dynamic window manager from suckless).

TODO: find out why dwm is not using my font, but dmenu is.

fancybarclickable
=================

I created the [fancybarclickable](http://dwm.suckless.org/patches/fancybarclickable) patch for dwm. It is based on [fancycoloredbarclickable](http://dwm.suckless.org/patches/fancycoloredbarclickable), which is based on [fancybar](http://dwm.suckless.org/patches/fancybar) and [statuscolors](http://dwm.suckless.org/patches/statuscolors). The fancybarclickable patch shows the window titles of all the windows in the current tag in the dwm bar, and it lets you select windows by selecting their title in the dwm bar.

In the first half of 2013, there was a huge dwm refactor. Unfortunately, the fancycoloredbarclickable, fancybar, and statuscolors patches are older than that and were affected by the refactor, so they no longer work.

I took the fancybar patch and updated it against [commit 3d1090b](http://git.suckless.org/dwm/commit/?id=3d1090ba896319368c4771b88d325fcee368a608), which was the latest version of dwm at the time. Then, I saw that fancycoloredbarclickable has a feature where you can click on window titles in the bar to select a window. I decided to include that feature in my patch.

I merely updated existing patches. Credits to the authors of the original patches:

1. Mate Nagy for fancybar
2. Stefan Mark for fancycoloredbarclickable

If anyone wants me to update the statuscolors patch, let me know. Naturally, if I update statuscolors, I'll also update fancycoloredbarclickable, since I already took care of the fancybarclickable part of that patch.

01-dwm.patch
============

01-dwm.patch is a patch of patches (what I like to call my quilt patch). It is patched against [commit 3d1090b](http://git.suckless.org/dwm/commit/?id=3d1090ba896319368c4771b88d325fcee368a608), which was the latest version of dwm at the time. It consists of:
* [fancybarclickable](http://dwm.suckless.org/patches/fancybarclickable) (written by me)
* [maximize](http://dwm.suckless.org/patches/maximize) (written by Jan Christoph Ebersbach)
* [moveresize](http://dwm.suckless.org/patches/moveresize) (written by Claudio M. Alessi and Jan Christoph Ebersbach)
* [multimon](http://dwm.suckless.org/patches/multimon) (written by Gary B. Genett)
* [swapfocus](http://dwm.suckless.org/patches/swapfocus) (written by Lasse Engblom and Jan Christoph Ebersbach)
* [viewontag](http://dwm.suckless.org/patches/viewontag) (written by Markus P.)

And it consists of some personal changes to config.h:
* font
* tagging rules
* resizehints
* MODKEY
* volume control
* screen locking
* keybindings
