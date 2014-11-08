Patches for dwm (dynamic window manager from suckless).

fancybarclickable
=================

I created the fancybarclickable patch for dwm. It is based on [fancycoloredbarclickable](http://dwm.suckless.org/patches/fancycoloredbarclickable), which is based on [fancybar](http://dwm.suckless.org/patches/fancybar) and [statuscolors](http://dwm.suckless.org/patches/statuscolors).

In the first half of 2013, there was a huge dwm refactor. Unfortunately, the fancycoloredbarclickable, fancybar, and statuscolors patches are older than that and were affected by the refactor, so they no longer work.

I took the fancybar patch and updated it against [commit 3d1090b](http://git.suckless.org/dwm/commit/?id=3d1090ba896319368c4771b88d325fcee368a608), which was the latest version of dwm at the time. Then, I saw that fancycoloredbarclickable has a feature where you can click on window titles in the bar to select a window. I decided to include that feature in my patch.

The fancybarclickable patch shows the window titles of all the windows in the current tag in the dwm bar, and it lets you select windows by selecting their title in the dwm bar.

I merely updated existing patches. Credits to the authors of the original patches:
1. Mate Nagy for fancybar
2. Stefan Mark for fancycoloredbarclickable

If anyone wants me to update the statuscolors patch, let me know. Naturally, if I update statuscolors, I'll also update fancycoloredbarclickable.
