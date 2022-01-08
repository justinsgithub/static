#  Basic Linux Commands


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

*** -rw-r--r-- 1 root root 32059 2017-04-03 11:05 oo-cd-cover.odf *** ( example ) 

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
