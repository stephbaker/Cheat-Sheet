# Command Line Cheat Sheet

<img width="257" alt="screen shot 2018-09-05 at 3 02 58 pm" src="https://user-images.githubusercontent.com/42748054/45115068-cc531e00-b11c-11e8-92cb-ec22b56b6df0.png">

### Tips
- Use the up and down arrows to toggle through your previous commands
- Options modify the behavior of commands.


## SHORTCUTS

| Key/Command | Description |
| ----------- | ----------- |
| Ctrl + A   | Go to the beginning of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + E   | Go to the end of the line you are currently typing on.  This also works for most text input fields system wide.  Netbeans being one exception |
| Ctrl + Q   | Clears everything on current line |
| Ctrl + L   | Clears the Screen |
| Cmd + K    | Clears the Screen |
| Ctrl + U   | Cut everything backwards to beginning of line |
| Ctrl + K   | Cut everything forward to end of line |
| Ctrl + W   | Cut one word backwards using white space as delimiter |
| Ctrl + Y   | Paste whatever was cut by the last cut command |
| Ctrl + H   | Same as backspace |
| Ctrl + C   | Kill whatever you are running |
| Ctrl + D   | Exit the current shell when no process is running, or send EOF to a the running process |
| Ctrl + Z   | Puts whatever you are running into a suspended background process. fg restores it. |
| Ctrl + _   | Undo the last command. (Underscore.  So it's actually Ctrl + Shift + minus) |
| Ctrl + T   | Swap the last two characters before the cursor |
| Ctrl + F   | Move cursor one character forward |
| Ctrl + B   | Move cursor one character backward |
| Option + →  | Move cursor one word forward |
| Option + ←  | Move cursor one word backward |
| Esc + T  | Swap the last two words before the cursor |
| Tab  | Auto-complete files and folder names |
| * | Select groups of files ( ex. m*.txt = selects all files in working directory starting with m and ending with .txt |


## COMMANDS

| Key/Command | Description |
| ----------- | ----------- |
| clear | clears the screen |
| ls | looks at the folder you are in and gives a short list |
| ls -a | Listing showing hidden files |
| ls -l | Listing all content in long format |
| ls -t | Listing in order of last modified|
| pwd | Stands for "Print working directory" outputs where you currently are | 
| cd [folder] | Brings you to a new directory "change directory" | 
| cd folder] /folder]  | navigate directly to a specific directory |
| cd .. | Moves up one directory (moves back one) |
| mkdir something | add a new directory named something " made directory" |
| touch | creates a new file in a directory | 
| touch [folder]/[file to create] | creates a file without changing directory |
| cp [file] [newfile] | copy file to new file | 
| cp [file] [dir] |	copy file to directory |
| mv [file] [dir] | moves files |
| mv [file] [newfilename] | renames file |
