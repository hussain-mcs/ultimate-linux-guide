# Understanding the Folder Structure

### Explanation of System Directories

### **Symbolic Links (Less Significant)**
| Directory | Description |
|-----------|-------------|
| `/sbin -> /usr/sbin` | System binaries for administrative commands (linked to `/usr/sbin`). |
| `/bin -> /usr/bin` | Essential user binaries (linked to `/usr/bin`). |
| `/lib -> /usr/lib` | Shared libraries and kernel modules (linked to `/usr/lib`). |
| /sbin	| Contains essential system binaries for root user (symlink to /usr/sbin).|
| /lib	| Shared libraries required by system programs (symlink to /usr/lib).|
| /boot	| Holds bootloader files like vmlinuz and initrd.|
| /bin	| Essential user command binaries (symlink to /usr/bin).|
| /usr	| Contains user-installed software and libraries.|
| /srv	| Holds data for services like web and FTP servers.|
| /mnt	| Mount point for temporarily mounted filesystems.|
| /media	| Mount point for external media like USB drives and CDs.|
| /var	| Variable files like logs, spools, and cache.|
| /data	| Custom directory often used to store application data.|
| /proc	| Virtual filesystem exposing kernel and process information.|
| /dev	| Contains device files for accessing hardware.|
| /sys	| Virtual filesystem for kernel, hardware, and system info.|
| /tmp	| Temporary files, usually cleared on reboot.|
| /root	| Home directory for the root user.|
| /test	| Custom directory, possibly for testing purposes.|
| /opt	| Optional software packages and third-party apps.|
| /run	| Runtime variable data like PID files and sockets.|
| /home	| Home directories for regular users.|
| /etc	| System-wide configuration files.|

### **Important System Directories**
| Directory | Description |
|-----------|-------------|
| `/boot` | Stores files needed for booting the system (not relevant in containers). |
| `/usr` | Contains most user-installed applications and libraries. |
| `/var` | Stores logs, caches, and temporary files that change frequently. |
| `/etc` | Stores system configuration files. |

### **User & Application-Specific Directories**
| Directory | Description |
|-----------|-------------|
| `/home` | Default location for user home directories. |
| `/opt` | Used for installing optional third-party software. |
| `/srv` | Holds data for services like web servers (rarely used in containers). |
| `/root` | Home directory for the root user. |

### **Temporary & Volatile Directories**
| Directory | Description |
|-----------|-------------|
| `/tmp` | Temporary files (cleared on reboot). |
| `/run` | Holds runtime data for processes. |
| `/proc` | Virtual filesystem for process and system information. |
| `/sys` | Virtual filesystem for hardware and kernel information. |
| `/dev` | Contains device files (e.g., `/dev/null`, `/dev/sda`). |

### **Mount Points**
| Directory | Description |
|-----------|-------------|
| `/mnt` | Temporary mount point for external filesystems. |
| `/media` | Mount point for removable media (USB, CDs). |
| `/data` | Likely your **mounted volume** from Windows (`C:/ubuntu-data`). |
