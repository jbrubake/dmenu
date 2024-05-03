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

- dmenu-borderoption-20200217-bf60a1e.diff
- dmenu-center-20200111-8cd37e1.diff
- dmenu-fuzzyhighlight-4.9.diff
- dmenu-lineheight-5.0.diff
- dmenu-listfullwidth-5.0.diff
- dmenu-xresources-4.9.diff (modified to include additional resources)
- dmenu-nosort-5.0.diff
- dmenu-password-5.0.diff (change mask character to `*` instead of `.`)
- Add a `make distclean` target to delete `config.h`
- Add support for color emojis

Stay Synced with Upstream
-------------------------

After cloning this repo, add the upstream repository as a remote:

    $ git remote add upstream "https://git.suckless.org/dmenu"

To merge changes from upstream:

    $ git fetch upstream
    $ git merge upstream/master

