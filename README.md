You can create a VBS file to run this powershell script. That way this will act as a toggle switch and you can bind that VBS file to mouse button.

Something like -
```vbs
Set oShell = CreateObject ("Wscript.Shell") 
Dim strArgs
strArgs = "cmd /c ""powershell C:\Users\nk981\Documents\toggle_mute.ps1"""
oShell.Run strArgs, 0, false
```
