## dev.eden_emu.eden

> [!NOTE]
> This package is not endorsed by Eden

Welcome! Before making an issue, please follow these steps:
- Eden is on the latest stable release
- My issue does NOT happen on the official AppImages
- I have not edited Eden's permissions
- My issue isn't in the known issues

If your issue happens on the official AppImages, please make an [issue here](https://github.com/eden-emulator/Issue-Reports/issues). \
If your issue happens only the flatpak build, make an issue in [this repo](https://github.com/flathub/dev.eden_emu.eden/issues). \
If you're having trouble with Discord RPC, see [this guide](https://github.com/flathub/com.discordapp.Discord/wiki/Rich-Precense-(discord-rpc)).

## How do I make my Eden app look 'nice'?'
This is a guide on how to theme Eden outside of KDE. Users on KDE can simply set the Qt widget style as Breeze, and pick whichever theme they want via the plasma settings.
- Set `XDG_CURRENT_DESKTOP=KDE` in your environment variables via flatseal. 
- If your Qt widget style is still fusion, set `QT_STLYE_OVERRIDE=Breeze` the same way as above.
- Configure your **kdeglobals** file to apply whatever theme you would like. For example, you could symlink /usr/share/color-schemes/BreezeDark.colors into ~/.config/kdeglobals.
- If you're on GNOME, Eden might not respect your theme settings. I have no idea why this is the case.
> [!NOTE]
> Editing **kdeglobals** could have unintended consequences that may affect other apps
