# AutoHotkey script to Open or Show Apps


This [AutoHotkey](https://www.autohotkey.com/) script is to Open, Restore or Minimize the desired Apps, using the shortcuts key (hotkeys) that you want to set.<br /> 
It works well with regular Window Apps, Windows Store Apps, Chrome Shortcuts and Chrome Apps.

There are three **utility functions** for this purpose:

**a)** `OpenOrShowAppBasedOnExeName(AppAddress)` - Useful for regular Window Apps

**b)** `OpenOrShowAppBasedOnWindowTitle(WindowTitleWord, AppAddress)` - Specially useful for Chrome Apps and Chrome Shortcuts 

**c)** `OpenOrShowAppBasedOnAppModelUserID(AppTitle, AppModelUserID)` - Useful for Windows Store Apps (contained in the "shell:AppsFolder\")
  

## Configuration Examples

`F7:: OpenOrShowAppBasedOnExeName("C:\Windows\System32\SnippingTool.exe")`

`F8:: OpenOrShowAppBasedOnWindowTitle("Gmail", "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe --app=https://mail.google.com/mail/")`

`F9:: OpenOrShowAppBasedOnAppModelUserID("Calculator", "Microsoft.WindowsCalculator_8wekyb3d8bbwe!App")`


## Installation Steps

1- Download and install the AutoHotkey App [here](https://www.autohotkey.com/)

2- Download the script file [here](https://github.com/JuanmaMenendez/AutoHotkey-script-Open-Show-Apps/releases/latest/download/AutoHotkey-script-Open-Show-Apps.ahk)

3- Edit the script (Notepad works) and create your shortcuts, setting your [keys](https://autohotkey.com/docs/KeyList.htm) and the address to your desired App by using the above utility functions

For example, this line `F7:: OpenOrShowAppBasedOnExeName("C:\Windows\System32\SnippingTool.exe")`  will open the Window's SnippingTool when you press the *F7* key

4- Execute the script (Double click on it)

5- (Optional) In order to automatically load this script on System Start Up, create a Window desktop shortcut for it and move it into the Windows startup folder, located exactly at "*%APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup*"

6- Enjoy


## Extras

### Switch between open windows of the same App / Type

Pressing **Alt + `** (key above Tab key) you wil be able to switch between open windows of the same App / Type (Eg: between multiple Chrome windows)


### Find AppModelUserID

To get the AppUserModelID of a Windows Store App, you can use this [comprehensive guide](https://jcutrer.com/windows/find-aumid).