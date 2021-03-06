# Command Line Cheat Sheet

<img width="257" alt="screen shot 2018-09-05 at 3 02 58 pm" src="https://user-images.githubusercontent.com/42748054/45115068-cc531e00-b11c-11e8-92cb-ec22b56b6df0.png">

### Tips
- Use the up and down arrows to toggle through your previous commands
- Options modify the behavior of commands.
- ~/.bash_profile is where settings are stored
- nano editor is a command line text editor


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
| Tab | Auto-complete files and folder names |
| wc | word count | 


## SYMBOLS

| Key/Command | Description |
| ----------- | ----------- |
| * | Select groups of files ( ex. m*.txt = selects all files in working directory starting with m and ending with .txt |
| ~ | represents home directory | 
| . | indicates hidden file | 
| $ | always used when returning a variable's value | 

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
| cd [folder] /[folder]  | navigate directly to a specific directory |
| cd .. | Moves up one directory (moves back one) |
| mkdir something | add a new directory named something " made directory" |
| touch | creates a new file in a directory | 
| touch [folder]/[file to create] | creates a file without changing directory |
| cp [file] [newfile] | copy file to new file | 
| cp [file] [dir] |	copy file to directory |
| mv [file] [dir] | moves files |
| mv [file] [newfilename] | renames file |
| rm [file] | deletes files |
| rm -r(f) [directory] | deletes directory |
| cat | outputs content of a file |
| less | similar to cat but better at holding bigger files | 
| tail -5 | prints the last 5 lines of something | 
| sort | alphabetizes input |
| uniq | filters out adjacent, duplicate lines (sort deserts.txt //| uniq) is effect to alphabetize and then filter |
| grep [word] [text] | "global regular expression print" and searches files for lines (careful it's case sensitive | 
| grep -i | allows command to be case insenitive | 
| grep -R[directory] | searches all files in a directory and outputs filenames ( -R  stands for "recursive") |
| grep -Rl | searches all files in a directory and outputs only filenames with matched results. |
| grep \ [string] - hr | FIGURE OUT WHAT H DOES |
| sed 's/[word]/[replacement word]/'[text] | "stream editor" and works like a find and replace (only for first instance of word | 
| sed 's/[word]/[replacement word]/g'[text] | g at the end means global and will replace all instances |
| nano[file] | opens a new text file "[writing]" is what's in the text and ^ starts for ctrl in the info bank |
| clear | clears the terminal | 
| nano ~/.bash_profile | opens up the profile | 
| echo "[words] | echo the string when a new terminal session begins | 
| source | activates the changes |
| alias [shortcut]="[original]" | create keyboard shortcuts | 

## ENVIRONMENT VARIABLES

| Key/Command | Description |
| ----------- | ----------- |
| export | makes variable availible to all child sessions | 
| PS1 | variable that defines the makeup style of the command prompt (export PS1=">> ") | 
| env | "environment", and returns a list of the environment variables for the current user ( PATH, PWD, PS1, HOME) ex. env \\| grep LESS| 

## DIRECTORY MANAGEMENT

| Key/Command | Description |
| ----------- | ----------- |
| [command] > [file]| Push output to file (note it overwrites what was already on the file) |
| [command] >> [file]	| Adds output to existing file |
|  \\| | "pipes" standard input to the command on left ($ cat volcanoes.txt \\| wc \\| cat > islands.txt) takes word count and pipes to cat then redirected to island |
| cat < | redirect standard input of something to cat | 
