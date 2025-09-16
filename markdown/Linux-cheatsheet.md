# Linux Command Line Cheatsheet (Enhanced)

## File & Directory Navigation
| Command | Action |
|---------|--------|
| pwd | Print working directory (show current path) |
| ls | List files in directory |
| ls -l | List files with details (permissions, size, date) |
| ls -a | List all files, including hidden |
| cd <dir> | Change directory |
| cd .. | Go up one directory |
| cd ~ | Go to home directory |
| tree | Display directories as a tree (if installed) |

---

## File Operations
| Command | Action |
|---------|--------|
| touch <file> | Create an empty file |
| cp <src> <dest> | Copy file |
| cp -r <src> <dest> | Copy directory recursively |
| mv <src> <dest> | Move or rename file/directory |
| rm <file> | Remove file |
| rm -r <dir> | Remove directory recursively |
| rm -rf <dir> | Force remove directory (⚠ dangerous) |
| file <file> | Show file type |
| stat <file> | Show detailed file info |

---

## Viewing & Editing Files
| Command | Action |
|---------|--------|
| cat <file> | Print file contents |
| less <file> | View file with scrolling |
| head <file> | Show first 10 lines |
| head -n 20 <file> | Show first 20 lines |
| tail <file> | Show last 10 lines |
| tail -f <file> | Continuously watch file (logs) |
| nano <file> | Edit file in nano |
| vim <file> | Edit file in Vim |

---

## User & System Info
| Command | Action |
|---------|--------|
| whoami | Show current user |
| id | Show user ID and groups |
| uname -a | Show system info |
| hostname | Show hostname |
| uptime | Show system uptime |
| date | Show current date/time |
| cal | Show calendar |
| free -h | Show memory usage |
| df -h | Show disk space usage |
| du -sh <dir> | Show size of directory |

---

## Process Management
| Command | Action |
|---------|--------|
| ps | Show running processes |
| ps aux | Show all processes with details |
| top | Interactive process viewer |
| htop | Better interactive viewer (if installed) |
| kill <pid> | Kill process by PID |
| kill -9 <pid> | Force kill process |
| pkill <name> | Kill process by name |
| jobs | Show background jobs |
| fg %n | Bring job `n` to foreground |
| bg %n | Resume job `n` in background |

---

## Permissions
| Command | Action |
|---------|--------|
| ls -l | Show permissions |
| chmod +x <file> | Make file executable |
| chmod 755 <file> | Set specific permissions |
| chown user:group <file> | Change file ownership |
| sudo <command> | Run command as superuser |

---

## Networking
| Command | Action |
|---------|--------|
| ip a | Show IP addresses |
| ifconfig | Show network interfaces (legacy) |
| ping <host> | Ping a host |
| curl <url> | Fetch data from URL |
| wget <url> | Download file from URL |
| ssh user@host | Connect to remote server via SSH |
| scp file user@host:/path | Copy file via SSH |
| netstat -tuln | Show open ports (legacy) |
| ss -tuln | Show open ports (modern) |

---

## Package Management
*(Depends on distro)*  
| Command | Action |
|---------|--------|
| apt update | Update package list (Debian/Ubuntu) |
| apt upgrade | Upgrade all packages |
| apt install <pkg> | Install package |
| apt remove <pkg> | Remove package |
| dnf install <pkg> | Install package (Fedora/RHEL) |
| pacman -S <pkg> | Install package (Arch) |
| yum install <pkg> | Install package (older RHEL/CentOS) |

---

## Archiving & Compression
| Command | Action |
|---------|--------|
| tar -cvf file.tar dir | Create tar archive |
| tar -xvf file.tar | Extract tar archive |
| tar -czvf file.tar.gz dir | Create compressed tar.gz archive |
| tar -xzvf file.tar.gz | Extract tar.gz archive |
| zip file.zip <files> | Create zip archive |
| unzip file.zip | Extract zip archive |

---

## Search & Find
| Command | Action |
|---------|--------|
| find /path -name <file> | Find file by name |
| grep "pattern" <file> | Search text in file |
| grep -r "pattern" <dir> | Search recursively |
| locate <file> | Find file (uses database, run `updatedb` first) |
| which <command> | Show path of command |
| whereis <command> | Show all locations of command |

---

## Shortcuts
| Shortcut | Action |
|----------|--------|
| Ctrl-c | Kill running process |
| Ctrl-z | Suspend process |
| fg | Resume last process in foreground |
| bg | Resume last process in background |
| !! | Run last command again |
| !<cmd> | Run last command starting with `<cmd>` |
| Tab | Autocomplete filename/command |
| Ctrl-r | Reverse search command history |
