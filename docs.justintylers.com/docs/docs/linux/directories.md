# Linux Directory Structure

## root directory ( / )


| directory | description |
| --------- | ----------- |
| / | the root directory where everything begins |
| /bin | contains binaries (programs) that must be present for the system to boot and run |
| /boot | contains the Linux kernel, initial RAM disk image (for drivers needed at boot time), and the boot loader |
| /dev | this is a special directory that contains device nodes | 
| /etc | directory contains all of the system-wide configuration files |
| /home | in normal configurations each user is given a directory here |
| /lib | contains shared library files used by the core system programs |
| /lost+found | used in the case of a partial recovery from a file system corruption event |
| /media | contains the mount points for removable media such as USB drives that are mounted automatically at insertion |
| /mnt | contains mount points for removable devices that have been mounted manually |
| /opt | used to install “optional” software commercial software products that might be installed on the system |
| /proc |  virtual file system maintained by the Linux kernel where the “files” it contains are peepholes into the kernel itself |
| /root | This is the home directory for the root account |
| /sbin | contains “system” binaries for programs that perform vital system tasks that are generally reserved for the superuser |
| /tmp | intended for the storage of temporary / transient files created by various programs |
| /usr | contains programs and support files used by regular users and executable programs installed by the Linux distribution |
| /usr/lib | The shared libraries for the programs in /usr/bin |
| /usr/local | where programs that are not included with the distribution but are intended for systemwide use are installed |
| /usr/sbin | Contains more system administration programs |
| /usr/share | /usr/bin programs shared data like default configuration files and screen backgrounds |
| /usr/share/doc | documentation files for installed packages |
| /var | directory tree where data that is likely to change such as log files are stored |
