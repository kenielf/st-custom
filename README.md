# Custom ST
*Note: This configuration is built entirely for my own usage.*

A fork of `st` with additional patches and configurations!

The original repository and information can be found [here](https://st.suckless.org/)

## Patches
 1. **[Alpha](https://st.suckless.org/patches/alpha/)** 
 [(Direct Link)](https://st.suckless.org/patches/alpha/st-alpha-20220206-0.8.5.diff)
 2. **[Glyph Wide Support](https://st.suckless.org/patches/glyph_wide_support/)** 
 [(Direct Link)](https://st.suckless.org/patches/glyph_wide_support/st-glyph-wide-support-20220411-ef05519.diff)
 3. **[Scrollback](https://st.suckless.org/patches/scrollback/)**
 [(Direct Link 1)](https://st.suckless.org/patches/scrollback/st-scrollback-20210507-4536f46.diff)
 [(Direct Link 2)](https://st.suckless.org/patches/scrollback/st-scrollback-mouse-20220127-2c5edf2.diff)

## Building and Installation
First, clone the repository and navigate to its folder with:
```bash
git clone "https://github.com/kenielf/st-custom"
cd st-custom
```

Then, build `st` with:
```bash
make st
```
*Note: `st` depends on `libx11` and `libxft`, alongside a C compiler like `gcc`!*

And lastly, install it with:
```bash
mkdir -p ~/.local/bin
ln -sfT $(pwd)/st ~/.local/bin/st
ln -sfT $(pwd)/st.desktop ~/.local/share/applications/st.desktop
```

Done, `st` should now be available as a command as long as `~/.local/bin` is 
part of your `PATH`.

## Original Readme
The original readme can be found [here](/README)
