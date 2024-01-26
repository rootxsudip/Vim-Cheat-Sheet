# Vim-Cheat-sheet

## Navigation Keys:
`j` - Used for going down  
`k` - Used for going up  
`h` - Used for going right  
`l` - Used for going left  
`2w` - To move the cursor two words forward  
`3e`  To move the cursor to the end of the third word forward  
`0` - To move the cursor to the start of the line  
`$` - To move the cursor to the end of the line  
`gg` - To move the cursor to start of the file  
`GG` - To move the cursor to end of the file  

## Text Editing
### Insertion and Appending Keys
`i`   - Turn on Insert mode for editing text  
`I`   - Turn on Insert mode for editing text at start of the line  
`o`   - Turn on Insert mode for editing text at next line  
`O`   - Turn on Insert mode for editing text at above line  
`esc` -  Turn on Normal mode  
`a` - Append at end of the line  
`a` - Append after a word  

### Save and Quit Keys
`:w` - Save  
`:w <filename>` - Save with filename  
`:wq` - Save and Quit  
`:q` - Quite  
`:q` - Quit without saving the file  
`ZZ` - Quickest way to save and exit  

### Deletion with motions(w,e,$)
`x` - Delete a character
`dw` - Delete until the start of the next word, EXCLUDING its first character  
`d2w` - Delete two words until the start of the next word, EXCLUDING its first character  
`de` - to the end of the current word, INCLUDING the last character  
`d$` - to the end of the line, INCLUDING the last character  
`dd` - Delete whole line  
`2dd` - Delete two lines  

### Undo
`u` - Undo the last commands  
`U` - Fix a whole line  
`CTRL-R` - Redo(undo the undos)  

### Copy and Put/Paste
`y` - Copy a highlighted text  
`yy` - Copy a line  
`p` - Put/Paste  
`dd` - Cut/Delete  

### Replace
`r<character>` - Enter the in replace mode and change character  
`R` - Replace mode is like Insert mode, but every typed character deletes an existing character  

### Change
`ce` - To change until the end of a word  
The change operator works in the same way as delete  
The format is:
`c [number] motion`

## Search
`/` - / followed by a text  
`n` - Search for the same text again  
`N` - Search for the same text again in the opposite direction  
`:set ic` - Enable Ignore case - It matches upper and lower  
`:set noic` - Disable Ignore case  
`CTRL-O` - To go back to where you came from  
`CTRL-I` - Goes forward
### Matching Parenthesis Search
Place the cursor on any (, [, or {  
`/<closing-parenthesis>` - Move the cursor to the other matching parenthesis

## Substitute
`:s/old/new` - To substitute new for the first old in a line type  
`:s/old/new/g` - To substitute new for all 'old's on a line type  
`:#,#s/old/new/g` - To substitute phrases between two line #'s type  
`:%s/old/new/g` - To substitute all occurrences in the file type  
`:%s/old/new/gc` - To ask for confirmation each time add 'c'  

## External Commands
`:!<sys-command>` - Run Extnernal Commands

## Selection
`v` - Selection  
`ggdG` - Select all lines and delete  

## Merger files
`:r<filename/command>` - Insert thhe output below the cursor  
