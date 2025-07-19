# W10-W11CleanInstall
Scripts/resources for EXPERIMENTAL Windows10/11 clean installation. Please refreain from using these for the time being.

## Screenshots will be added for documenting the changes.
When I have the time...

## What is this repository?
This repo (will) contains scripts/resources for clean, bloatfree, and customized Windows 10/Windows 11 installations.

### Using Memory's [UnattendedWinstall](https://github.com/memstechtips/UnattendedWinstall) answer file as a base;
  * Integrated [FR33THY's Remove Edge script](https://github.com/FR33THYFR33THY/Ultimate-Windows-Optimization-Guide/blob/main/6%20Windows/14%20Edge.ps1) - will remove Edge upon installation. No fuss.
  * Wrote a utility to install MY favourite (see below) software(s) using winget. This tool will also repair winget if it's not available for a reason. (Which happens in W10 - idk)
  * Added "Open File Location", "Open cmd here" and "Open powershell here" to right click context menu - without needing to press shift.
  * Added "Create .cpp and .hpp file" option to right click context menu - I'm a C++ programmer.
  * Changed default "wallpaper" to black. (No wallpaper)
  * Enabled some options which original disables:
    * File size information in folder tips
    * Pop-up description for folder and desktop items
    * Status bar
    * Taskbar animations
    * Translucent selection rectangle
    * Drop shadows for icon labels on desktop
  * Set taskbar buttons to show labels and never combine
  * Removed JPEG wallpaper quality limit.
  * Apply Black + #ffcf48 dark mode color theme. (No explorer patch, just colors)
  * Taskbar will be set to left instead of middle.
  * Taskbar Search bar will not be removed, instead will be made an icon.
  * Taskview button on Taskbar will not be hidden.
  * Added two cursor sets. You can browse them at [W10-W11CleanInstall/Resources/Cursors/](https://github.com/aeris170/W10-W11CleanInstall/Resources/Cursors). Default cursor will be [Obsidian](https://www.deviantart.com/teft/art/Obsidian-Cursor-set-78972293) by [teft](https://www.deviantart.com/teft/gallery).
  * ... and possibly other stuff I failed to remember. Nothing malicious. You should still diff the original with mine. You can use an online tool or use a program like Meld.
> [!WARNING]  
> Definitely diff! No one but you is responsible if your break anything. We will laugh at you if you break your setup and come complaining in the issues!

### How to use?
  Follow [UnattendedWinstall](https://github.com/memstechtips/UnattendedWinstall).
> [!IMPORTANT]
Please make sure you have internet during installation. Resources folder will be downloaded.

> [!TIP]
If you can't/won't have internet druing installation, you can launch "Download Resources" from desktop after logging in.

### License - usage rights?
  Use this in any way you desire. You must give credit to [Memory](https://github.com/memstechtips), [FR33THY](https://github.com/FR33THYFR33THY), [catppuccin](https://github.com/catppuccin). If you are able to, also give credit to [aeris170 (me)](https://github.com/aeris170).

#### YOUR Favoutire Software(s)?
> [!NOTE]
The list below is planned to be the final list — tentative. The current autoattend.xml does not include all those below. autoattend.xml includes some other programs unmentioned below. This will be fixed soon.

Yes, all via winget 😏 you have the option to select which. Don't like some? Don't install those.
  * **7zip**
  * **Auto Hotkey**
  * **Battle.net**
  * **Blender**
  * **CMake**
  * **Crystal Disk Info**
  * **Discord**
  * **EarTrumpet**
  * **Filelight**
  * **Flameshot**
  * **Flawless Widescreen**
  * **Flow Launcher**
  * **GIMP**
  * **Git**
> [!NOTE]  
> Git will be installed in "interactive mode". Make sure to have your "favourite" text editor installed.
  * **GitHub Desktop**
  * **Google Chrome**
  * **Google Drive**
  * **HiBit Uninstaller**
  * **HWiNFO**
  * **ImageGlass (Image Viewer)**
  * **LibreWolf**
  * **Line 6 Central**
  * **Microsoft Office**
  * **Modern Flyouts**
  * **NanaZip (7zip modern UI fork)**
  * **Neofetch**
  * **Nilesoft Shell**
> [!IMPORTANT]
> Nilesoft comes with it's own Terminal tab. Thefore CMD and pwsh options will have duplicates. You can run
> ```
> regedit /S C:\Windows\Setup\Scripts\TidyContextMenu.reg
> ```
> to clean-up context menu.

> [!TIP]
> You can also apply my own custom changes very easily:
>  * A matching theme (edited [catppuccin mocha yellow](https://github.com/catppuccin/nilesoft-shell))
>  * Cleaned-up context menu
>  To apply, run:
>  ``` 
>  powershell C:\Windows\Setup\Scripts\ApplyNilesoftConfig.ps1
>  ```
> 
>  * You will need to Ctrl+Rightlick Desktop to apply changes
  * **Notepad++**
  * **OBS Studio**
  * **Oracle VM Virtual Box**
  * **Paint.NET**
  * **PDFgear**
  * **PowerToys**
  * **PuTTY (SSH Client)**
  * **Python 3.13**
  * **qBittorrent**
  * **Rainmeter**
  * **RenderDoc**
  * **Runescape 3**
  * **Screenbox**
  * **Sourcetree**
  * **Spicetify (Spotify Themer)**
  * **Spotify**
  * **Steam**
  * **Sucrose Wallpaper Engine**
  * **TcNo Account Switcher**
  * **TeraCopy**
  * **UniGetUI (Winget UI)**
  * **Visual Studio 2022**
  * **WinDirStat**
  * **Windhawk**
> [!TIP]
> You can apply my preferred mods very easily:
>   * Always show all taskbar tray icons
>   * Middle click to close on the taskbar
>   * Modernize Folder Picker Dialog
>   * Slick Window Arrangement
>   * Taskbar Clock Customization - Two Lines Format:
>     * **Monday 15:28:29**
>     * **Dec 09.12.2024**
>   * Taskbar on top for Windows 11
>   * Taskbar tray system icon tweaks
>     * Hide Battery, GPS, Language bar, Bell
>   * To apply, run:
>   ```
>   powershell C:\Windows\Setup\Scripts\ApplyWindhawkConfig.ps1
>   ```
>   * You may need to restart Windhawk
  * **WinSCP (FTP Client)**
  * **Zettlr (Markdown Editor)**