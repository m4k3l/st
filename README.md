# st - simple terminal
My build of st, a simple terminal emulator for X which sucks less.

Forked from [suckless](https://git.suckless.org/st).


## Patches
The following patches have been applied:

- [boxdraw](https://st.suckless.org/patches/boxdraw)
- [glyph wide support](https://st.suckless.org/patches/glyph)
- [scrollback](https://st.suckless.org/patches/scrollback)
- [font2](https://st.suckless.org/patches/font2)
- [alpha](https://st.suckless.org/patches/alpha)


## Requirements
In order to build st you need the Xlib header files.


## Installation
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):
```
make
sudo make install
```


## Running st
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```
tic -sx st.info
```

See the man page for additional details.

## Credits
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.
