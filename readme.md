# YABST

## Introduction
YABST (Yet another Bash script template) is a skeleton for bash scripts. It has several gloal functions (all starting with "_") to help structuring your code. Standard parameters like help, version or the quite mode flag are built-in.

## Installation
Simply download the yabst file and modify it to your own needs.


## Global Functions
**_config**
Evaluate the file ($1) as a list of commands, executed in the current context. Usage is reading variables in config files like `/etc/lsb-release`.

**_echo**
Displays a message ($1) if the quite mode flag is set to false.

**_error**
Displays a error message ($1) and exit the program.

**_replace**
Replace in a file ($1) some string ($2) with another string ($3).

**_root**
Checks if the current user root, if not the program is terminated.

**_title**
Displays a headline ($1) enclosed by stars and a blank linke before and after.

**_usage**
Displays the comment part at the beginning of the script.

**_version**
Displays the current script version.

**_write**
Write the content ($1) to a file ($2 or 'out.txt' if $2 is empty).

## License
YABST is released under the [MIT license](https://github.com/teotiger/yabst/blob/master/license.txt).

## Version History
Version 1.1 - January 11, 2017
* new functions (_replace and _write)

Version 1.0 – November 11, 2016
* Initial release
