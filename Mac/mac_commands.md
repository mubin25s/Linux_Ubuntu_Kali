# macOS Command Reference

This guide provides a comprehensive list of essential macOS terminal commands for file management, system administration, networking, and development.

## 1. File & Directory Management
| Command | Description |
| :--- | :--- |
| `ls` | List directory contents |
| `cd <dir>` | Change directory |
| `pwd` | Print working directory |
| `cp <src> <dest>` | Copy files or directories |
| `mv <src> <dest>` | Move or rename files or directories |
| `rm <file>` | Remove files or directories |
| `mkdir <name>` | Create a new directory |
| `touch <file>` | Create an empty file or update timestamps |
| `cat <file>` | Display file content |
| `open <file>` | Open a file, directory, or application |
| `pbcopy` / `pbpaste` | Copy/Paste data to/from the clipboard |
| `find <dir> -name <p>` | Search for files in a directory |
| `locate <name>` | Find files by name using a database |

## 2. System Information & Processes
| Command | Description |
| :--- | :--- |
| `sw_vers` | Print macOS operating system version |
| `system_profiler` | Detailed hardware and software configuration |
| `hostinfo` | Display host information |
| `top` | Display real-time process information |
| `ps aux` | Report status of all running processes |
| `kill <pid>` | Terminate a process by ID |
| `killall <name>` | Force quit an application by name |
| `uptime` | See how long the system has been running |
| `caffeinate` | Prevent the system from sleeping |

## 3. Application & Utility Management
| Command | Description |
| :--- | :--- |
| `open -a <app>` | Launch a specific application |
| `installer -pkg <p> -target /` | Install a .pkg file via CLI |
| `softwareupdate -l` | List available software updates |
| `softwareupdate -ia` | Install all available software updates |
| `say "<text>"` | Convert text to speech |
| `screenshot -c` | Take a screenshot to the clipboard |
| `mdls <file>` | List Spotlight metadata for a file |

## 4. Networking
| Command | Description |
| :--- | :--- |
| `ifconfig` | Display network interface parameters |
| `networksetup` | Configure network settings |
| `ping <host>` | Send ICMP ECHO_REQUEST to network hosts |
| `traceroute <host>` | Trace the route packets take to a host |
| `netstat` | Display network status and statistics |
| `nslookup` / `dig` | DNS lookup utilities |
| `curl <url>` | Transfer data from or to a server |
| `lsof -i` | List active network connections |

## 5. Disk Management
| Command | Description |
| :--- | :--- |
| `diskutil list` | List all disks and partitions |
| `df -h` | Display free disk space (human-readable) |
| `du -sh <dir>` | Estimate file space usage for a directory |
| `mount` / `umount` | Mount/Unmount a file system |
| `hdiutil mount <dmg>` | Mount a disk image (.dmg file) |
| `fsck` | File system consistency check and repair |

## 6. Permissions & Security
| Command | Description |
| :--- | :--- |
| `sudo <command>` | Execute a command with admin privileges |
| `chmod <mode> <file>`| Change file/directory permissions |
| `chown <user> <file>`| Change file/directory ownership |
| `ls -ale` | List files with ACLs and detailed permissions |
| `csrutil status` | Check System Integrity Protection (SIP) status |
| `security` | Administer certificates and keychains |

## 7. Package Management (Homebrew)
| Command | Description |
| :--- | :--- |
| `brew install <pkg>` | Install a package |
| `brew update` / `upgrade`| Update Homebrew and upgrade packages |
| `brew list` | List all installed packages |
| `brew search <text>` | Search for packages |
| `brew doctor` | Check system for potential problems |

## 8. Developer Tools
| Command | Description |
| :--- | :--- |
| `xcode-select --install`| Install Command Line Tools |
| `zsh` | The default macOS shell |
| `env` | Display current environment variables |
| `alias <name>='<cmd>'`| Create command shortcuts |
| `python3` / `pip3` | Python runtime and package manager |
| `node` / `npm` | Node.js runtime and package manager |
| `nano` / `vim` | Built-in text editors |
