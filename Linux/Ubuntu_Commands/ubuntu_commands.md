# Ubuntu Command Reference

This guide provides a comprehensive list of essential commands for Ubuntu Linux, covering file management, package handling, system administration, and security.

## 1. Terminal Basics
| Command | Description |
| :--- | :--- |
| `clear` | Clear the terminal screen |
| `exit` | Close the terminal session |
| `history` | Show command history |

## 2. File & Directory Management
| Command | Description |
| :--- | :--- |
| `ls -la` | List all files in detail (including hidden) |
| `pwd` | Show current directory path |
| `cd <dir>` | Change directory |
| `mkdir <name>` | Create a new directory |
| `rmdir <name>` | Delete an empty directory |
| `touch <file>` | Create an empty file |
| `cp <src> <dest>` | Copy file or directory (`-r` for recursive) |
| `mv <src> <dest>` | Move or rename file/directory |
| `rm <file>` | Delete a file |
| `rm -rf <dir>` | Force delete a directory (⚠ Use with caution) |

## 3. File Viewing & Editing
| Command | Description |
| :--- | :--- |
| `cat <file>` | Display entire file content |
| `less <file>` | View content with pagination |
| `head <file>` | Show first 10 lines |
| `tail <file>` | Show last 10 lines |
| `tail -f <file>` | Live log view (continuous output) |
| `nano <file>` | Simple terminal text editor |
| `vim <file>` | Advanced terminal text editor |

## 4. Package Management (APT)
| Command | Description |
| :--- | :--- |
| `sudo apt update` | Update package lists |
| `sudo apt upgrade` | Upgrade all installed packages |
| `sudo apt install <pkg>`| Install a new package |
| `sudo apt remove <pkg>` | Remove a package |
| `sudo apt autoremove` | Clean up unused dependencies |
| `apt search <query>` | Search for a package |
| `apt show <pkg>` | Show detailed package information |

## 5. Snap Package Management
| Command | Description |
| :--- | :--- |
| `snap find <query>` | Search for snap packages |
| `snap install <pkg>` | Install a snap package |
| `snap remove <pkg>` | Remove a snap package |
| `snap list` | List installed snap packages |
| `snap refresh` | Update all snap packages |
| `snap info <pkg>` | Show detailed information about a package |
| `snap revert <pkg>` | Revert to previous version |

## 6. System & Process Monitoring
| Command | Description |
| :--- | :--- |
| `top` / `htop` | Real-time system monitoring |
| `ps aux` | List all running processes |
| `kill <pid>` | Terminate a process by ID |
| `df -h` | Display disk space usage |
| `free -h` | Display RAM usage |
| `uptime` | System running time |

## 7. Systemd Service Management (systemctl)
| Command | Description |
| :--- | :--- |
| `systemctl start <svc>` | Start a service |
| `systemctl stop <svc>` | Stop a service |
| `systemctl restart <svc>`| Restart a service |
| `systemctl status <svc>`| Check service status |
| `systemctl enable <svc>`| Enable service on boot |
| `systemctl disable <svc>`| Disable service on boot |
| `systemctl daemon-reload`| Reload systemd configuration |

## 8. Networking & Firewall (UFW)
| Command | Description |
| :--- | :--- |
| `ip addr` | View IP addresses and interfaces |
| `ping <host>` | Test network connection |
| `sudo ufw enable` | Enable UFW firewall |
| `sudo ufw status` | Check firewall status |
| `sudo ufw allow <port>` | Allow traffic on a port |
| `sudo ufw deny <port>` | Block traffic on a port |
| `sudo ufw reload` | Reload firewall rules |

## 9. Disk Maintenance
| Command | Description |
| :--- | :--- |
| `lsblk` | List block devices and partitions |
| `fdisk -l` | List partition tables |
| `du -sh <dir>` | Disk usage of a directory |
| `df -h` | Display free disk space |
| `mount <dev> <pt>` | Mount a filesystem |
| `umount <pt>` | Unmount a filesystem |
| `fsck <dev>` | Check and repair filesystem |
| `blkid` | Show block device UUIDs |

## 10. Archive & Compression
| Command | Description |
| :--- | :--- |
| `tar -cvf <file.tar> <dir>` | Create a tar archive |
| `tar -xvf <file.tar>` | Extract a tar archive |
| `zip <file.zip> <file>` | Create a zip file |
| `unzip <file.zip>` | Extract a zip file |

## 11. Search & Find
| Command | Description |
| :--- | :--- |
| `find . -name "<name>"` | Find files by name |
| `grep "<text>" <file>` | Search for text in a file |
| `grep -r "<text>" .` | Recursive text search |

## 12. User & Permissions
| Command | Description |
| :--- | :--- |
| `whoami` | Show current user |
| `sudo <command>` | Run command with admin privileges |
| `chmod +x <file>` | Make file executable |
| `chmod 755 <file>` | Set standard permissions |
| `chown <user> <file>` | Change file owner |

## 13. Logs & Troubleshooting
| Command | Description |
| :--- | :--- |
| `journalctl` | Query systemd journal |
| `journalctl -u <svc>` | Show logs for a specific service |
| `journalctl -f` | Follow log output in real-time |
| `dmesg` | Show kernel boot messages |
| `last` | Show last logged in users |
| `tail -f /var/log/syslog`| Follow system log file |
