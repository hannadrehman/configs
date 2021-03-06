# Usefull vim commands


## 1. Basic Vim commands#
The most simple commands allow you to open and close documents as well as saving them. As with most other text editors, there are protections in place to help you avoid exiting the editor without having saved what you’re working on.

`:help [keyword]` - Performs a search of help documentation for whatever keyword you enter

`:e [file]` - Opens a file, where [file] is the name of the file you want opened

`:w` - Saves the file you are working on

`:w [filename]` - Allows you to save your file with the name you’ve defined

`:wq` - Save your file and close Vim

`:q!` - Quit without first saving the file you were working on

## 2. Vim commands for movement

`h` - Moves the cursor to the left

`l` - Moves the cursor to the right

`j` - Moves the cursor down one line

`k` - Moves the cursor up one line

`H` - Puts the cursor at the top of the screen

`M` - Puts the cursor in the middle of the screen

`L` - Puts the cursor at the bottom of the screen

`w` - Puts the cursor at the start of the next word

`b` - Puts the cursor at the start of the previous word

`e` - Puts the cursor at the end of a word

`0` - Places the cursor at the beginning of a line

`$` - Places the cursor at the end of a line

`o` - insert new line below and go to insert mode

`O` - insert new line below and go to insert mode

`)` - Takes you to the start of the next sentence

`(` - Takes you to the start of the previous sentence

`}` - Takes you to the start of the next paragraph or block of text

`{` - Takes you to the start of the previous paragraph or block of text

`Ctrl + f` - Takes you one page forward

`Ctrl + b` - Takes you one page back

`gg` - Places the cursor at the start of the file

`G` - Places the cursor at the end of the file

`#` - Where # is the number of a line, this command takes you to the line specified

`ctrl + d` (scroll window downwards, normally half a a screen)

`ctrl + u` (scroll window upwards, normally half a a screen)

## 3. Vim commands for editing

`yy` - Copies a line

`yw` - Copies a word

`y$` - Copies from where your cursor is to the end of a line

`v` - Highlight one character at a time using arrow buttons or the h, k, j, l buttons

`V` - Highlights one line, and movement keys can allow you to highlight additional lines

`p` - Paste whatever has been copied to the unnamed register

`d` - Deletes highlighted text

`dd` - Deletes a line of text

`dw` - Deletes a word

`D` - Deletes everything from where your cursor is to the end of the line

`d0` - Deletes everything from where your cursor is to the beginning of the line

`dgg` - Deletes everything from where your cursor is to the beginning of the file

`dG` - Deletes everything from where your cursor is to the end of the file

`x` - Deletes a single character

`u` - Undo the last operation; u# allows you to undo multiple actions

`Ctrl + r` - Redo the last undo

`.` - Repeats the last action

## 4. Vim commands for searching text

`/[keyword]` - Searches for text in the document where keyword is whatever keyword, phrase or string of characters you’re looking for

`?[keyword]` - Searches previous text for your keyword, phrase or character string

`n` - Searches your text again in whatever direction your last search was

N - Searches your text again in the opposite direction

`:%s/[pattern]/[replacement]/g` - This replaces all occurrences of a pattern without confirming each one

`:%s/[pattern]/[replacement]/gc` - Replaces all occurrences of a pattern and confirms each one

## 5. Vim commands for working with multiple files

`:bn` - Switch to next buffer

`:bp` - Switch to previous buffer

`:bd` - Close a buffer

`:sp [filename]` - Opens a new file and splits your screen horizontally to show more than one buffer

`:vsp [filename]` - Opens a new file and splits your screen vertically to show more than one buffer

`:ls` - Lists all open buffers

`Ctrl + ws` - Split windows horizontally

`Ctrl + wv` - Split windows vertically

`Ctrl + ww` - Switch between windows

`Ctrl + wq` - Quit a window

`Ctrl + wh` - Moves your cursor to the window to the left

`Ctrl + wl` - Moves your cursor to the window to the right

`Ctrl + wj` - Moves your cursor to the window below the one you’re in

`Ctrl + wk` - Moves your cursor to the window above the one you’re in

## 6. Marking text (visual mode)

`v` - starts visual mode, you can then select a range of text, and run a command V - starts linewise visual mode (selects entire lines) Ctrl + v - starts visual block mode (selects columns) ab - a block with () aB - a block with {} ib - inner block with () iB - inner block with {} aw - mark a word Esc - exit visual mode

Once you’ve selected a particular range of text, you can then run a command on that text such as the following:

`d` - delete marked text y - yank (copy) marked text > - shift text right < - shift text left ~ - swap case (upper or lower)

## 7. Insert Mode (i)

`<Esc>` or `CTRL-C` exit insert mode

`CTRL-H` - Delete the character before the cursor

`CTRL-W` - Delete the word before the cursor

`CTRL-U` - Delete all entered characters in the current line

`CTRL-J` - Begin new line

`CTRL-N` - Find next keyword

`CTRL-P` - Find previous keyword

`CTRL-T` - shift entire line to next indent

`CTRL-D` - delete 1 indent in entire line

`CTRL-E` - scroll window one line up.

`CTRL-Y` - scroll window one line down.

`<S-Left>` -	cursor one word back (like "b" command)	 

`<C-Left>` -	cursor one word back (like "b" command)	

`<S-Right>` -	cursor one word forward (like "w" command)

`<C-Right>` -	cursor one word forward (like "w" command)



## text objects around

sa{motion/textobject}{addition}. For example, a key sequence saiw( makes foo to (foo).

sd{deletion}. For example, key sequences sdb or sd( makes (foo) to foo. sdb searches a set of surrounding automatically.

sr{deletion}{addition}. For example, key sequences srb" or sr(" makes (foo) to "foo".

## commenter

[count]<leader>cc |NERDCommenterComment|

[count]<leader>c<space> |NERDCommenterToggle|

[count]<leader>cs |NERDCommenterSexy|
 
CTRL-o. opens last file

CRTl-i opens next file 

% matches the closing tag,bracket etc

## Code folding

zf{%} collaps code blocks matching closing bracket

za opens folded code block

=i{ fixes indentation inside { brackets
