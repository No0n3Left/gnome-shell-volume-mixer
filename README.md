GNOME Shell Volume Mixer
========================


Shell Volume Mixer is an extension for GNOME Shell allowing separate
configuration of PulseAudio devices and output switches. It features a profile
switcher to quickly switch between pinned profiles and devices.

Middle mouse click on a slider mutes the selected stream.


![screenshot 1](/screenshot_1.png?raw=true "Outputs menu") ![screenshot 2](/screenshot_2.png?raw=true "Inputs menu")



Installation
------------

```
$ make
```

That's it. Add the resulting archive via GNOME Tweak Tool (extensions tab) or
copy it's content manually to
".~/.local/share/gnome-shell/extensions/shell-volume-mixer@derhofbauer.at".


GNOME Settings Daemon (GSD)
---------------------------

GSD hardcodes the step for each key press of volume keys to 6% of maximum
volume. While this might be OK for most people, some would prefer a
configurable setting. There's a bug in GNOME's tracker which, according to the
comments by developers, won't ever get fixed in a way that could allow
configurable volume
steps<sup>[[1]](https://bugzilla.gnome.org/show_bug.cgi?id=650371)</sup>.

Shell Volume Mixer tries to grab GSD's hotkeys to provide configurable steps
for sliders and media keys.


Acknowledgments
---------------

This is a fork of AdvancedVolumeMixer by Harry Karvonen
(git://repo.or.cz/AdvancedVolumeMixer.git).
Many thanks go out to him for his initial work.
