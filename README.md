# A [pywal](https://github.com/dylanaraps/pywal) compatible fork of st

## Patches applied

- Alpha OSC 11
- Anysize
- Xresources
- Scrollback ringbuffer
- Boxdraw
- Ligatures boxdraw
- Bold is not bright
- Desktop entry
- Netwmicon

## Other changes

- Changed key bindings for zooming in/out
- Added key bindings for scrolling
- Changed default color definitions

*Check the manual for key bindings.*

## Dependencies

- fontconfig
- libX11
- libXft
- harfbuzz
- libgd

*Make sure that appropriate header files are installed too.*

## Installation

```shell
git clone https://github.com/tokatatahan/st
cd st
sudo make clean install
```

## Uninstallation

```shell
sudo make uninstall
```

## Configuration

Configuration is done via editing `config.h` and then recompiling. If this file
does not exist, it will be automatically generated. Automatically generated
file will be a copy of `config.def.h` and it will be owned by the root user. If
you mess something up, or apply a new patch that changes `config.def.h`, you
should run the following command:

```shell
cp config.def.h config.h
```

**This will overwrite the existing `config.h`!**
