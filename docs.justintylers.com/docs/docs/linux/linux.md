# Linux 

> content also applies to many unix like operating system's

## directories 


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


## ls 

|       variation       |                 description                       |
| --------------------- | ------------------------------------------------- |
| ls                    | list files in a directory                         |
| -a / --all            | List all files including hidden files             |
| -A / --almost-all     | like the -a option above except it does not list . and .. |
| -d / --directory      | use with -l to see details about the directory rather than its contents |
| -F / --classify       | append an indicator character to the end of each listed name | 
| -h / --human-readable | display file sizes in human readable format rather than in bytes |
| -l                    | Display results in long format                    |
| -r / --reverse        | Display the results in reverse alphabet order     |
| -S                    | Sort results by file size                         |
| -t                    | Sort by modification time                         |

### ls -l fields

*** -rw-r--r-- 1 root root 32059 2017-04-03 11:05 oo-cd-cover.odf ***

*** -rw-r--r--  ***

    - access rights to the file
    - the first character indicates the type of file
    - a leading dash means a regular file
    - “d” indicates a directory 
    - the next three characters are the access rights for the file's owner
    - the next three are for members of the file's group
    - the final three are for everyone else

*** 1  *** = File's number of hard links

*** root   *** = The username of the file's owner

*** root   *** = The name of the group that owns the file

*** 32059   *** = Size of the file in bytes

*** 2007-04-03 11:05  *** = Date and time of the file's last modification

*** oo-cd-cover.odf  *** = Name of the file

## cd 

> change directories

| variation | result | 
| -------- | ---- |
| cd | changes the working directory to your home directory |
| cd - | changes the working directory to the previous working directory | 
| cd ~ user_name | changes the working directory to the home directory of user_name |


## less 

> view a files content

|      Command       |     Action      |
| ------------------ | --------------- |
| Page Up or b       | Scroll back one page |
| Page Down or space | Scroll forward one page |
| Up arrow           | Scroll up one line |
| Down arrow         | Scroll down one line |
| G                  | Move to the end of the text file |
| 1G or g            | Move to the beginning of the text file |
| /characters        | Search forward to the next occurrence of characters |
| n                  | Search for the next occurrence of the previous search |
| h                  | Display help screen |
| q                  | Quit less |

## touch 

create a new file

## date

display date

## cal 

displays current month calendar

## df

current amount of free space on disk drive 

## free 

amount of free memory 

## exit 

> or Ctrl-d

end terminal session

## pwd 

print path to working directory

## file 

determine a file type

## cp 

copy files and directories

## mv 

move/rename files and directories

## mkdir 

create directories

## rm 

remove files and directories

## ln 

create hard and symbolic links

## Sed

> stream editor 

### double space lines in file 

```shell
sed  '/^$/d;G'
```
## zsh

> the z shell

### my current prompt

```zsh
PS1="%F{yellow}%~ %F{red} =%F{yellow}(%#)%F{red}=> "

RPS1="%F{green}%D %F{white}%T %F{red}%n%{$reset_color%}@%F{blue}%m %h%F{yellow} %Bjobs%b %j"
```

<div class="termy">
```console
<span style='color:red;'>=</span><span style='color:yellow;'>(%)</span><span style='color:red;'>=></span> echo 'RPS1 not featured here ):'
```
</div>

### zsh  loop

```zsh
for x in 1 2 3 4 5 6 7 8 9; echo $x
```
