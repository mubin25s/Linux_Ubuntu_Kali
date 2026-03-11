# Arch Linux Command Reference

This guide provides a comprehensive list of essential commands for Arch Linux, covering package management (Pacman/AUR), system maintenance, and network configuration.

## 1. Terminal Basics
| Command | Description |
| :--- | :--- |
| `clear` | Clear the terminal screen |
| `exit` | Close the terminal session |

## 2. Package Management (Pacman)
| Command | Description |
| :--- | :--- |
| `sudo pacman -Syu` | Update database and upgrade all packages |
| `sudo pacman -S <pkg>` | Install a new package |
| `sudo pacman -R <pkg>` | Remove a package |
| `sudo pacman -Rs <pkg>` | Remove package and its dependencies |
| `sudo pacman -Rns <pkg>`| Remove package, dependencies, and configs |
| `sudo pacman -Ss <key>` | Search for a package |
| `sudo pacman -Qi <pkg>` | Show detailed package info |
| `sudo pacman -Qdt` | List orphaned packages |
| `sudo pacman -Qdtq` | List orphaned packages (quiet mode) |
| `sudo pacman -U <file>` | Install local package (.pkg.tar.zst) |
| `sudo pacman -Sc` | Clean package cache |
| `sudo pacman -Scc` | Clean entire package cache |

## 3. AUR Helpers (Yay / Paru)
| Command | Description |
| :--- | :--- |
| `yay -S <pkg>` | Install from AUR using Yay |
| `paru -S <pkg>` | Install from AUR using Paru |
| `yay -Syu` | Upgrade system and AUR packages |
| `yay -Ss <key>` | Search repositories and AUR |

## 4. Manual AUR Installation
To install a package from the AUR manually:
1. `git clone https://aur.archlinux.org/<pkg>.git`
2. `cd <pkg>`
3. `makepkg -si` (Build and install dependencies)

## 5. Arch Build System (ABS)
| Command | Description |
| :--- | :--- |
| `makepkg` | Build package from PKGBUILD |
| `makepkg -si` | Build and install with dependencies |
| `makepkg -src` | Build and clean up source files |
| `updpkgsums` | Update checksums in PKGBUILD |
| `namcap <file>` | Check PKGBUILD for errors |
| `asp checkout <pkg>` | Retrieve source PKGBUILD for official package |

## 6. System Maintenance
| Command | Description |
| :--- | :--- |
| `reflector --latest 5` | Update mirrorlist with fastest mirrors |
| `paccache -r` | Remove all but last 3 cached versions |
| `timedatectl set-ntp true`| Sync system time with network |
| `hostnamectl set-hostname`| Change system hostname |
| `pacman -Rns $(pacman -Qdtq)`| Remove all orphaned packages recursively |
| `rm /var/lib/pacman/db.lck`| Remove pacman lock file |

## 7. Network Configuration
| Command | Description |
| :--- | :--- |
| `ip link` | Show network interfaces |
| `ip addr` | Show IP addresses |
| `nmcli device wifi list`| List available Wi-Fi networks |
| `nmcli device wifi connect <SSID> password <PWD>` | Connect to Wi-Fi |
| `nmtui` | Text-based interface for NetworkManager |
| `iwctl` | Interactive Wi-Fi configuration tool |

## 8. Disk Management (Arch Specific)
| Command | Description |
| :--- | :--- |
| `cfdisk <dev>` | Simple partition editor |
| `fdisk <dev>` | Advanced partition editor |
| `lsblk -f` | List block devices and filesystems |
| `mkfs.ext4 <part>` | Format partition to ext4 |
| `mkfs.fat -F32 <part>`| Format partition for EFI/boot |
| `genfstab -U /mnt >> /etc/fstab`| Generate fstab file |
| `arch-chroot /mnt` | Change root for repair/install |

## 9. Logs & Troubleshooting
| Command | Description |
| :--- | :--- |
| `journalctl -p 3 -xb` | Show errors from current boot |
| `journalctl -f` | Follow logs in real-time |
| `systemctl --failed` | List all failed services |
| `dmesg \| grep -i error`| Search kernel ring buffer for errors |
| `checkupdates` | Check for updates without syncing |
