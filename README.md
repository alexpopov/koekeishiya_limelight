## Limelight

**IMPORANT:** This project is not maintained and uses and outdated technique to attempt to sync external border windows to the windows owned by other applications running on the system.
This was created because borders were removed from the yabai project at the time. Since then, a new and improved border system has been implementend, which supercedes this project.

**README:** https://github.com/koekeishiya/limelight/issues/37

--

Port of the old border system that used to be implemented in yabai v2.4.3.

For the old version of limelight that was simply a focused border, see [focused_border_only](https://github.com/koekeishiya/limelight/tree/focused_border_only)

Requires access to the accessibility API. Supports macOS High Sierra, Mojave, Catalina and Big Sur.

Documentation: https://github.com/alexpopov/koekeishiya_limelight/blob/master/doc/limelight.asciidoc

```sh
# add the following to the end of your yabairc to have it launch automatically when yabai starts.
# make sure the limelight binary is added somewhere in your $PATH

# kill any existing limelight process if one exists, before we launch a new one
killall limelight &> /dev/null
limelight &> /dev/null &
```

### Build

Requires xcode command line tools

```sh
# simply clone repo and run make
  make

# symlink binary to somewhere in your path (does not need to be re-created after a rebuild)
# replace the second argument below with some directory in your path
  ln -s /path/to/bin/limelight /usr/local/bin/limelight
```
