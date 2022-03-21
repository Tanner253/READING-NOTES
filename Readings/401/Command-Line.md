# THE TERMINAL

## The command line

- The command line or terminal is a text based interfaceing system to the computer. You enter commands and your response from the terminal will be in text format.

## Basic Navigation

- We can find where we are in the file structure with PWD (Print working dirtectory)

- ls allows us to see all of the public files in the directory while ls -a will unhide hidden files. ls - l will give a thurough detailed list of all of the contents in the directory.

- Paths : absolute and relative. Absolute paths specify location in relation from the root. whereas relative will specify the location in relation to where we currently are. ~ = home . = current directory .. = parent directory

- Files : Linux is case sensitive. you can cd into directories or select directories with a space by puting the file name in quotes. you can also use an escape character .... \

- Manual pages descirbe every command available on your system and details what they do. use the man keyword to trigger manual pages. the syntax is man "< command >" which will return the manual related to that specific command to help troubleshoot.
  the man pages are your friend.

- make a new directory with the mkdir keyword, you can also remove a directory with rmdir but the directory must be empty. you can create a new file with the touch keyword. you can use the cp keyword to copy a file and move it to another location, we can then specify the location for the file or directory to be copied too.

- we can move a directory with the mv keyword, specifying the source directory and the desired directory destination

- deleting directories with files: rm dir -r the -r notes this is a recursive command meaning run the command on evey thing inside the directory.

- Text editor : the keyword vi will bring up the text editor, vi < file name > will bring up the text editor on a specific file. once you open the text editor switch to "insert mode" by pressing i. pressing escape will end the file change.
  ZZ: save and exit | q!: discard changes since last save and exit| w: save file but dont exit | wq: save and exit.

- use keyword cat to see the contents of a file however if the file is humongous then use the 'less' keyword. less allows you to move up and down within a file using the arrow keys. You may go forward a whole page using the SpaceBar or back a page by pressing b. When you are done you can press q for quit.
- VI COMMANDS: Arrow keys - move the cursor around
  - j, k, h, l - move the cursor down, up, left and right (similar to the arrow keys)
  - ^ (caret) - move cursor to beginning of current line
  - $ - move cursor to end of the current line
  - nG - move to the nth line (eg 5G moves to 5th line)
  - G - move to the last line
  - w - move to the beginning of the next word
  - nw - move forward n word (eg 2w moves two words forwards)
  - b - move to the beginning of the previous word
  - nb - move back n word
  - { - move backward one paragraph
  - } - move forward one paragraph
- VI DELETE COMMANDS:
  - x - delete a single character
  - nx - delete n characters (eg 5x deletes five characters)
  - dd - delete the current line
  - dn - d followed by a movement command. Delete to where the movement command would have taken you. (eg d5w means delete 5 words)
  - U Will undo changes

## CHEAT SHEET
[CHEAT SHEET](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)
