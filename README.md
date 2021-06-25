dmenu - dynamic menu
====================
dmenu is an efficient dynamic menu for X.


Requirements
------------
In order to build dmenu you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install


Running dmenu
-------------
See the man page for details.

Patches Applied
---------------

- dmenu-border-4.9.diff
- dmenu-center-20200111-8cd37e1.diff
- dmenu-lineheight-5.0.diff
- dmenu-listfullwidth-5.0.diff
- dmenu-nosort-5.0.diff
- dmenu-xresources-4.9.diff (modified to include additional resources)

