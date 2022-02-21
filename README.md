# ITCommands
A collection of IT related commands that I have to google twice a month
---
## PowerShell
**Get PC boot-up history**
```powershell
Get-WinEvent -ProviderName Microsoft-Windows-Kernel-boot -MaxEvents 10 | Where-Object {$_.id -eq "27"} | select -ExpandProperty TimeCreated
```
