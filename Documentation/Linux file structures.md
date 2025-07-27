# Linux File Structures

**/** : The **root** of the filesystem. All other folders are under this. 

**/bin** : "Binary" executables essential for **basic system functionality**, like ls, cp, mv, bash. Used in both normal and rescue mode. 

**/sbin** : Like /bin, but for **system administration** tools (ifconfig, reboot, mount). Usually for root only. 

**/lib** : Shared **libraries** needed by /bin and /sbin.

**/lib64** : 64-bit versions of the libraries.

**/boot** : Contains **boot loader files**, like the Linux kernel vmlinuz, intrid and GRUB configs. 

**/dev** : Devices files - everything in Linux is a file, including disks /dev/sda, USBs, terminals, etc.

**/etc** : System-wide configuration files. No binaries, just config: /etc/password, /etc/hosts, /etc/ssh.

**/home** : User directories: /home/"user". Stores user data and settings.

**/media** : Mount point for removable data (USBs, CDs). Usually auto-mounted here.

**/mnt** : Temporary mount point for manual mounts (mounting a disk image).

**/proc** : Virtual filesystem exposing process and kernel information. /proc/cpuinfo, /proc/1234. 

**/sys** : Another virtual filesystem for hardware and system info (used with udev or kernel modules). 

**/run** : Temporary runtime data, like PID files or socket files. Creayed fresh at each boot. 

**/srv** : "Service" data. Used by services like FTP, HTTP, etc. Not always used in modern distros.

**/var** : Variable data: logs (/var/log/), spools, temporary emails, caches. 

**/tmp** : Temporary files: Often cleared on reboot. Apps use it for short-lived files.

**/usr** : Contains most user-installed software and libraries (think "unix system resources"). Subdirs include: 

- /usr/bin : non-essential binaries
- /usr/sbin : non-essential system binaries
- /usr/lib : libraries for /usr/bin and /usr/sbin
- /usr/local : manuallt compiled/installed software (not from package manager)

**/opt** : "optional" software. third party packages (often big ones like google chrome, VMware, etc.)

## Graphic structure

<img width="1817" height="1001" alt="image" src="https://github.com/user-attachments/assets/e96f5270-0e63-425b-b142-fafb01057074" />

## Mnemonic

"Every Big Server Lets Robots Eat Hard Metal Pipes Securely"

E = /etc 

B = /bin 

S = /sbin 

L = /lib

R = /root 

E = /etc 

H = /home 

M = /mnt

P = /proc

S = /sys 















