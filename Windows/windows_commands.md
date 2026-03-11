# Windows Command Reference

This guide provides a comprehensive list of essential Windows commands for Command Prompt (CMD) and PowerShell, covering system administration, file management, and networking.

## 1. File & Directory Management (CMD)
| Command | Description |
| :--- | :--- |
| `dir` | List directory contents |
| `cd <path>` | Change directory |
| `copy <src> <dest>` | Copy files |
| `del <file>` | Delete files |
| `move <src> <dest>` | Move or rename files |
| `mkdir <name>` | Create a new directory |
| `rmdir <name>` | Remove a directory |
| `ren <old> <new>` | Rename a file or directory |
| `type <file>` | Display text file content |
| `tree` | Graphical display of directory structure |

## 2. System Information & Management
| Command | Description |
| :--- | :--- |
| `systeminfo` | Detailed system configuration |
| `hostname` | Display computer name |
| `ver` | Display Windows version |
| `tasklist` | List all running processes |
| `taskkill /IM <name>`| Terminate a process by name |
| `taskmgr` | Open Task Manager (GUI) |
| `powercfg` | Configure power settings |
| `driverquery` | List installed device drivers |

## 3. Networking
| Command | Description |
| :--- | :--- |
| `ipconfig /all` | Detailed network configuration |
| `ping <host>` | Test connectivity to a host |
| `tracert <host>` | Trace the path to a destination |
| `nslookup <domain>` | Query DNS records |
| `netstat -an` | Display active network connections |
| `getmac` | Display MAC addresses of adapters |
| `netsh advfirewall` | Manage Windows Firewall |

## 4. Disk Management
| Command | Description |
| :--- | :--- |
| `diskpart` | Interactive disk partition manager |
| `chkdsk <drive> /f` | Check and repair disk errors |
| `format <drive>` | Format a disk |
| `defrag <drive>` | Consolidate fragmented files |
| `label` / `vol` | Manage volume labels and serial numbers |

## 5. Diagnostic & Recovery
| Command | Description |
| :--- | :--- |
| `sfc /scannow` | Repair corrupted system files |
| `dism /online /cleanup-image /restorehealth` | Repair the Windows image |
| `gpupdate /force` | Refresh Group Policy settings |
| `chkdsk /f /r` | Check disk and repair errors/locate bad sectors |
| `eventvwr` | Open Event Viewer (GUI) |
| `perfmon` | Open Performance Monitor (GUI) |

## 6. Security & Firewall
| Command | Description |
| :--- | :--- |
| `netsh advfirewall` | Manage Windows Firewall settings |
| `sc query` | Display status of system services |
| `icacls` | Display or modify Access Control Lists (ACLs) |
| `net share` | Manage shared resources |
| `cipher` | Display or alter encryption on NTFS volumes |
| `certutil` | Manage certificates and services |

## 7. User Management
| Command | Description |
| :--- | :--- |
| `whoami` | Display current user information |
| `whoami /priv` | Display current user privileges |
| `net user <name>` | Add, delete, or modify user accounts |
| `net localgroup` | Add, display, or modify local groups |
| `runas /user:<name>` | Run a program as another user |

## 8. PowerShell Basics (Cmdlets)
| Cmdlet | Description |
| :--- | :--- |
| `Get-Command` | List all available commands |
| `Get-Help <cmd>` | Show help for a command |
| `Get-Service` | List system services |
| `Get-Process` | List running processes |
| `Get-Content <file>` | Read file content |
| `Select-String` | Find text in strings and files |
| `Start-Process` / `Stop-Process` | Manage processes in PowerShell |
| `Invoke-WebRequest` | Fetch content from the web |
| `Set-ExecutionPolicy`| Change script execution policy |
| `Get-History` | Show command history for session |
