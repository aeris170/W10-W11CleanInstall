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
  * ... and other stuff I fail to remember at the moment. Nothing malicious. You should still diff the original with mine. You can use an online tool or use a program like Meld.

> [!WARNING]
Please make sure you have internet during installation. Resources folder will be downloaded. If they couldn't be downloaded during installation, launch "Download Resources" from desktop.

### How to use?
  Follow [UnattendedWinstall](https://github.com/memstechtips/UnattendedWinstall).

### License - usage rights?
  Use this in any way you desire. You must give credit to [Memory](https://github.com/memstechtips), [FR33THY](https://github.com/FR33THYFR33THY), [catppuccin](https://github.com/catppuccin). If you are able to, also give credit to [aeris170 (me)](https://github.com/aeris170).

#### YOUR Favoutire Software(s)?
> [!INFO]
The list below is planned to be the final list. The current autoattend.xml does not include all those below. autoattend.xml includes some other programs unmentioned below. This will be fixed soon.

Yes, all via winget 😏 you have the option to select. Don't like some? Don't install those.
  * **7zip**
  * **Auto Hotkey**
  * **Battle.net**
  * **Blender**
  * **CMake**
  * **Discord**
  * **FanControl**
  * **Flameshot**
  * **Flawless Widescreen**
  * **GIMP**
  * **Git**
  * **GitHub Desktop**
  * **Google Drive**
  * **HiBit Uninstaller**
  * **HWiNFO**
  * **Runescape**
  * **K-Lite Codec Pack Mega**
  * **Libre Office**
  * **LibreWolf**
  * **Line 6 Central**
  * **Microsoft Teams**
  * **Neofetch**
  * **Nilesoft Shell**
	* To remove excess Powershell and CMD buttons, run C:\Windows\Setup\Scripts\RemoveCMD_Pwsh.reg
	* To apply my custom changes with a matching theme (edited [catppuccin mocha yellow](https://github.com/catppuccin/nilesoft-shell)), run
    ```
    powershell C:\Windows\Setup\Scripts\ApplyNilesoftConfig.ps1 # (this will remove excess buttons)
    ```
	* You will need to Ctrl+Rightlick Desktop to apply changes
  * **Notepad++**
  * **NVCleanstall**
  * **Paint.net**
  * **PowerToys**
  * **PuTTY (SSH Client)**
  * **qBittorrent**
  * **Rainmeter**
  * **Razer Synapse 3**
  * **RenderDoc**
  * **Signal**
  * **Skype**
  * **Slack**
  * **Sourcetree**
  * **Spotify**
  * **Steam**
  * **SteelSeries GG**
  * **Stream Deck**
  * **TcNo Account Switcher**
  * **Teracopy**
  * **Thunderbird**
  * **Tor Browser**
  * **Visual Studio 2022**
  * **Oracle VM Virtual Box**
  * **WinDirStat**
  * **Windhawk**
    * My preferred mods:
      * Always show all taskbar tray icons
      * Middle click to close on the taskbar
      * Modernize Folder Picker Dialog
      * Slick Window Arrangement
      * Taskbar Clock Customization - Two Lines Format:
        * **Monday 15:28:29**
        * **Dec 09.12.2024**
      * Taskbar on top for Windows 11
      * Taskbar tray system icon tweaks
        * Hide Battery, GPS, Language bar, Bell
    * To apply my preferred mods and their settings, run
    ```
    powershell C:\Windows\Setup\Scripts\ApplyWindhawkConfig.ps1
    ```
    * You may need to restart Windhawk
  * **WinSCP (FTP Client)**