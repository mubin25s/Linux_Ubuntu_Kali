# Kali Linux Command Reference

This guide provides a comprehensive list of essential security and penetration testing commands for Kali Linux, covering information gathering, vulnerability analysis, and exploitation.

## 1. Terminal Basics
| Command | Description |
| :--- | :--- |
| `clear` | Clear the terminal screen |
| `exit` | Close the terminal session |

## 2. Information Gathering
| Command | Description |
| :--- | :--- |
| `nmap -v -A <ip>` | Full network scan with OS detection and scripts |
| `netdiscover -r <rng>` | Discover live hosts on the local network |
| `fping -asg <rng>` | Ping sweep to discover live hosts |
| `theHarvester -d <dom>`| Gather emails and subdomains from public sources |
| `dnsenum <dom>` | Comprehensive DNS enumeration |
| `whois <dom>` | Query WHOIS database for domain info |
| `whatweb <url>` | Identify technologies used by a website |

## 3. Vulnerability Analysis
| Command | Description |
| :--- | :--- |
| `nikto -h <url>` | Web server vulnerability scanner |
| `sqlmap -u <url>` | Automate SQL injection testing |
| `lynis audit system` | Perform a security audit of the local system |
| `nmap --script vuln <ip>`| Scan for known vulnerabilities using Nmap |
| `msfconsole` | Launch the Metasploit Framework |

## 4. Web Application Analysis
| Command | Description |
| :--- | :--- |
| `burpsuite` | Graphical web security testing proxy |
| `gobuster dir -u <url>` | Brute-force directories and files |
| `dirb <url> <list>` | Web content scanner |
| `wpscan --url <url>` | WordPress vulnerability scanner |
| `sqlmap -u <url> --dbs` | Enumerate databases via SQL injection |

## 5. Exploitation Tools
| Command | Description |
| :--- | :--- |
| `msfvenom -p <pay>` | Create malicious payloads |
| `beef-xss` | Browser Exploitation Framework |
| `hydra -l <u] -P <l> <ip>`| Online password cracking (SSH, FTP, etc.) |
| `searchsploit <term>` | Search the Exploit Database |
| `setoolkit` | The Social-Engineer Toolkit |
| `john <hashfile>` | John the Ripper hash cracker |
| `hashcat` | GPU-based hash cracker |

## 6. Wireless Attacks
| Command | Description |
| :--- | :--- |
| `iwconfig` | View wireless interfaces |
| `airmon-ng start <if>` | Enable monitor mode on interface |
| `airodump-ng <if>` | Capture wireless packets |
| `aireplay-ng <if>` | Perform packet injection |
| `aircrack-ng <file>` | Crack WPA/WPA2/WEP keys |
| `reaver -i <if> -b <bs>`| Attack WPS PINs |

## 7. Sniffing & Spoofing
| Command | Description |
| :--- | :--- |
| `wireshark` | GUI network protocol analyzer |
| `tshark -i <if>` | CLI packet capture |
| `bettercap -iface <if>`| Advanced network attack tool (MITM) |
| `ettercap -T -q -i <if>`| ARP poisoning attack (text mode) |
| `responder -I <if>` | LLMNR, NBT-NS, and MDNS poisoner |
| `tcpdump -i <if>` | Dump traffic on a network |
| `macchanger -r <if>` | Randomize MAC address |

## 8. Password Attacks
| Command | Description |
| :--- | :--- |
| `john <hashfile>` | Crack hashes using John the Ripper |
| `hashcat -m <md> <hsh>` | Advanced GPU hash cracking |
| `medusa -h <target>` | Parallel network login auditor |
| `ncrack` | High-speed network authentication cracker |
| `crunch <min> <max>` | Generate custom wordlists |
| `fcrackzip` | Crack password-protected ZIP files |

## 9. Forensics & Reverse Engineering
| Command | Description |
| :--- | :--- |
| `binwalk <file>` | Analyze and extract firmware images |
| `autopsy` | GUI for digital forensics |
| `volatility -f <file>` | Memory forensics framework |
| `strings <file>` | Extract printable characters from binaries |
| `radare2 <file>` | Advanced hex editor and debugger |
| `steghide extract -sf` | Extract hidden data from media |
| `pdfid <file.pdf>` | Scan PDF for malicious content |

## 10. Social Engineering
| Command | Description |
| :--- | :--- |
| `setoolkit` | The Social-Engineer Toolkit |
| `evilginx2` | Phishing framework for session cookies |
| `swaks` | Swiss Army Knife for SMTP (Email spoofing) |

## 11. Package Management (APT - Kali)
| Command | Description |
| :--- | :--- |
| `sudo apt update` | Update package database |
| `sudo apt full-upgrade`| Recommended way to upgrade Kali |
| `sudo apt install <pkg>`| Install a tool |
| `sudo apt search <pkg>` | Search for a security tool |
| `sudo apt show <pkg>` | Show package details |
