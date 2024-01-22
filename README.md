# Custom ST
*Note: This configuration is built entirely for my own usage.*

## Patches
 1. **[Alpha](https://st.suckless.org/patches/alpha/)** 
 [(Direct Link)](https://st.suckless.org/patches/alpha/st-alpha-20220206-0.8.5.diff)
 2. **[Glyph Wide Support](https://st.suckless.org/patches/glyph_wide_support/)** 
 [(Direct Link)](https://st.suckless.org/patches/glyph_wide_support/st-glyph-wide-support-20220411-ef05519.diff)

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
