Windows 10 Virtual Desktop Enhancer
===

This application enhances the Windows 10 virtual desktops feature.
By default you can only switch to the next/previous desktops by pressing [Windows + Ctrl + (Left or Right Arrow)].
This allows you to switch directly to each specific desktop on demand with new keyboard shortcuts.
It also allows you to have a custom wallpaper per desktop.

## Installation

For this app to work, you first might need to install "Visual C++ Redistributable for Visual Studio 2015".
It should be available [here](https://www.microsoft.com/en-us/download/details.aspx?id=48145).

This app does not need to be installed, simply extract it into a folder in your computer.

To run this app, just run the "virtual-desktop-enhancer.exe" program.

Alternatively you can install AutoHotkey and run the "virtual-desktop-enhancer.ahk" script file.

This application only works on Windows 10 x64.

## Troubleshooting

If the new keyboard shortcuts do not work and the tray icon doesn't update when changing desktops, install the optional patch (it might still not work, this has to do with the version of the runtimes that you have installed).

## Usage

### Keyboard Shortcuts

While running, the following keyboard shortcuts are available:
- [Left Alt + (key under Esc)]

    Goes to the desktop management screen.
    This is additionally available (by default) by pressing [Windows + Tab].
    You can move windows between desktops by dragging them while inside this screen.

- [Left Alt + (0-9)]

    Switch to the desktop for the respective key (ex: [LAlt + 3] goes to Desktop 3 and [LAlt + 0] goes to Desktop 10).

Note that to add a new desktop you can press the "New Desktop (+)" button on the desktop management screen.
A maximum of 10 desktops are supported.

### Tray Icon

A new tray icon will be available. It indicates the number of the current desktop (1-10).
If you click on it the desktop management screen is displayed.

The icons have white text over black background. Other icon themes are also available.

To change between them, go into the "icons" folder and extract the ZIP file for the theme you want to use, and replace any existing files if prompted. You can also use custom icons, by copying them into this folder and renaming them "1.ico" through "10.ico".

### Custom Wallpapers Per Desktop

To configure the wallpapers, edit the "settings.ini" file.
For each desktop, you can either set the wallpaper to be an image file or a fixed color.
To use images, set the path of the image, either absolute or relative (ex: "1=C:\wallpapers\1.jpg", "2=./wallpapers/2.jpg").
To use fixed colors, set the color in hexadecimal (ex: "3=0xff0000" for red, "4=0xff00" or "4=0x00ff00" for green).
If you set the config of that desktop to empty (ex: "5=") the wallpaper won't change when you switch to that desktop.

### Additional Configuration

You can also set what is the default desktop using the "[General] DefaultDesktop" setting.

## Credits

Thanks to Ciantic (Jari Pennanen) for his library and sample AHK script, which can be found [here](https://github.com/Ciantic/VirtualDesktopAccessor).
Thanks to the creator of the ReadINI AHK library, found [here](https://autohotkey.com/board/topic/33506-read-ini-file-in-one-go/).
Thanks to rob3110 on reddit for the extra white icon theme.
Thanks to the artists that created the packed wallpapers, whom I lost track of. Sorry.