A copy of the [st](https://st.suckless.org/patches/scrollback/) terminal
emulator repository including my configuration and patches I use.

Running `build.sh` resets the repository, applies the patches and builds st.

Build an install an Arch Linux package like this:
```sh
makepkg -sif PKGBUILD
```

Used patches:

* [scrollback](https://st.suckless.org/patches/scrollback/)

Some info about my configuration:

* [gruvbox](https://github.com/gruvbox-community/gruvbox) color scheme
  * using the color definition header from here:
    https://github.com/gruvbox-community/gruvbox-contrib/blob/master/st/gruvbox-dark.h
* Hack Nerd Font
  * https://www.nerdfonts.com/
  * https://sourcefoundry.org/hack/
  * https://aur.archlinux.org/packages/nerd-fonts-hack/
