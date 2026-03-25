
Tuxedo T. Penguin: A Quest for Herring.
========================================

                        The Original Game by Steve Baker
                           <sjbaker1@airmail.net>
                           http://www.woodsoup.org/~sbaker

(modified/unoriginal modded section begin)

Controls (More at ./docs/keystrokes.html):
--------
if you wanna use keyboard for tux movement, follow these steps:
1. press [space]
2. press View button
3. choose No Mousetrap button
4. press F1 for keymaps


### for mousetrappers(default):
- press right mouse button to stop tux

### for cheaters:
- self-explanatory



FAQ: 
------------

Q:whats the difference between the original and this?

A:the most answer is this mod is MOSTLY PLAYABLE and NO TOO MUCH SPEEDUPS (press z in-game for fastforward) + no need to modify Makefile thats just created by ./configure


Q:how to swim?

A:kindly hold the r or j button until tux is fully submerged. Then "move" forward and press the h button repeatedly 

Q: i see a very long warning text

A: ok, this is kinda technical but the point is that the engine to use OpenGL (GLUT) currently doesnt fully support a window manager called wayland. You're not doomed yet, you can always look the internet to switch it to Xorg/X11 or just pray and hope this game will switch to SDL/GLFW.

Q: its very laggy

A: it is, to accommodate the game speed.

Q: my tux always moving diagonally

A: well, the current solution is:

1. press [space]
2. press View button
3. choose No Mousetrap button

Q:keyboard mapping are weird

A:yes, i know that, at the future i'll remap those to something similiar like Project64

Q:what's the license for assets?

A:basically GPLv2, except the music (yes?) because it is from many websites with unclear license (including the mod archive iirc)

Q:does the gameplay follows the story?

A:it will, but not now.

(modified/unoriginal modded section end)



Installation:
--------------

Installation instructions are pretty basic,
and are covered in the documentation directory 'doc'.

First make sure that you have the following packages
installed:

- OpenGL (or Mesa) + GLIDE (if yuo have a 3Dfx card)
- GLUT (the GL Utility Toolkit)
- PLIB (which can be obtained from:
  http://www.woodsoup.org/projs/plib)

Once that is done, it should be a simple matter of changing
to the directory where all this stuff is unpacked and type:

(modified/unoriginal modded section begin)

 ```
 ./configure
 make
 ```

Do not... do not do `sudo make install`.. (or yes if you wanna make it an app thats still called tux_aqfh)

run the game:
```
./src/tux_aqfh
```
(modified/unoriginal modded section end)

However, you might want to check the full documentation -
especially if you need to install Mesa/GLIDE/GLUT before
you can start.

All documents are in HTML - so view them with your web browser.



License:
---------
This software is released under the provisions of
the GNU General Public License (GPL) which can be
found in the file 'LICENSE' in the current directory.



Directory Structure:
----------------------
- src     -- Where the source code lives.

- data    -- This contains all kinds of miscellaneous data
           files. Right now, this is limited to the level
           description files.

- doc     -- Documentation - all in HTML

- images  -- Texture maps and other images needed by the
           game. These are currently all in 'SGI' image
           format.

- models  -- 3D models used in the game. These are currently
           all in AC3D format - that decision may change
           at some time in the future.

- penguin -- The images and 3D models that make up Tux
           himself.

- wavs    -- Sound files - mostly sound effects.

- mods    -- MOD format music files.

(modified/unoriginal modded section below)



TODO:
-----
- switch to SDL (or GLFW)
- test and fix Windows port
- custom keymap
- clear save file location


Who made this README.md?
-----
its derived from the original README by Steve Baker, with additional modifications
