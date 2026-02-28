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

- dmenu-borderoption-20200217-bf60a1e.diff : 
- dmenu-center-20250407-b1e217b.diff : centers dmenu in the middle of the screen
- dmenu-fuzzyhighlight-5.3.diff : highlight the fuzzy matching characters of item
- dmenu-lineheight-5.0.diff : adds a '-h' option, which sets the minimum height of a dmenu line
- dmenu-listfullwidth-5.0.diff : vertical lists use full width instead of indenting items
- dmenu-nosort-5.0.diff : adds the -S option to disable sorting menu items after matching
- dmenu-password-5.0.diff : dmenu will not directly display the keyboard input, but instead replace it with dots (local change: set mask character to `*` instead of `.`)
- dmenu-xresources-4.9.diff : adds the ability to configure dmenu via Xresources

Local Changes
-------------

- dmenu-password : set mask character to `*` instead of `.`
- dmenu-xresources: include additional resources
- Add a `make distclean` target to delete `config.h`
- Add support for color emojis

Stay Synced with Upstream
-------------------------

After cloning this repo, add the upstream repository as a remote:

    $ git remote add upstream "https://git.suckless.org/dmenu"

To merge changes from upstream:

    $ git fetch upstream
    $ git merge upstream/master

