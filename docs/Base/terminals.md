# Terminals and Editors

## Terminals

In Linux world(MacOS as well) there is only one main terminal. It is command line interface.

![Macos terminal][macos]

[macos]: https://scrimba.com/articles/content/images/2022/07/macOS-terminal-04.png  "macos"

In MacOS(name of Operation system for Macbook) terminal application can be found in "Application" folder or in bottom panel of icons

![Macos app][mac-app]

[mac-app]: https://www.howtogeek.com/wp-content/uploads/2020/07/terminal_in_utilities_folder_2.png?trim=1,1&bg-color=000&pad=1,1 "mac-app"

## There are several editors

They are allow to edit content of files in Linux/MacOS like notepad.
All editors below work only with **plain text** format(simple text, no formatting like in Word). 

- vi (vim)
- nano
- gedit (grafical editor)

###  VI(VIM)

**Vi** is a  main and the  most popular editor which is available in every linux like operation system.

Usage example:

Step 1. create new text file(testfile.txt) and start editing

From terminal execute:

```
vi testfile.txt
```

and Tap <Enter>

Step 2. Tap ESC + i to start modifing the file

!!! note "VI restrictions"

    Editor supports cursor moving(array buttons) and erasing charachers(delete button)
    But ***vi*** doesnt support mouse cursor moving like in Word

When you tap ESC + i you will see status of editor in a bottom of a vi screen
Like this (-- INSERT --) line

![vi insert][insert]

[insert]: https://i.ytimg.com/vi/YpCFTy3c6Ic/maxresdefault.jpg "insert"

If you don't see such status, check the keyboard language(must be eng)


Step 3. To exit from editor Tap ESC + :wq and <Enter>

Step 4. To show content of any text file use **cat** linux command

```
cat testfile.txt
```

VIM is enchanced version of vi editor(same hot keys) and highlight syntax like this

![vim][vim]

[vim]: https://fuzeservers.ru/wp-content/uploads/a/c/3/ac39bd81e1ecd79329e7693a96f2e005.png "vim"


### Nano

Nano is second popular editor and doesnt require to be learnt

### Gedit

Gedit is grafical editor and can be used only if Linux server has grafical interface(where we can use mouse cursor and icons in Desktop).

All Linux servers don't have Grafical interface(because it consumes resources). All admins use only temninal mode in linux.

## Useful Links

* [Vi editor hot keys](https://www.atmos.albany.edu/daes/atmclasses/atm350/vi_cheat_sheet.pdf)
* [Russian article about vi](https://docs.altlinux.org/ru-RU/archive/2.3/html-single/junior/alt-docs-extras-linuxnovice/ch02s10.html)

