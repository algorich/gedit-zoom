Zoom - gedit plugin
===================

This plugin for gedit - GNOME text editor - adds the ability to change the
font size using either the menu bar, keyboard shortcuts or *<Ctrl>+mousewheel*
in a same manner as Firefox, OpenOffice and other applications.

Install
-------

Download the file *gedit-zoom-version.tar.gz* and extract the package into the
*~/.gnome2/gedit/plugins* directory, or - for a system-wide deployment - into
*/usr/lib/gedit-2/plugins* (the path may be different, depending on your
distribution).

Then activate and configure the plugin through Edit -> Preferences -> Plugins.

Development
-----------

It proved helpful for development to check out the git-repository to your
favorite location and create symlinks in your personal plugins directory to
the necessary files and directories. There is a make target, that accomplishes
this::

$ make install-dev

Authors
-------

Hugo Maia Vieira <hugomaiavieira@gmail.com> forked this from
http://github.com/dinkel/gedit-zoom developed by Christian Luginbühl
<dinkel@pimprecords.com>.

License
-------

See the LICENSE file.

Todo
----

If the font size is changed through Edit -> Preferences -> Font & Colors, then
these changes are not yet recognized by this plugin. Therefore changing the
zoom level still calculates with the fontsize when gedit was last started.
Restarting gedit fixes this annoyance.
