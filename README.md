# Vim

>Disclaimer: This cheatsheet is made for me to use. The reason I have this public is so someone else find it useful.

Command | Description 
:-- | :--
:w | write (save) the file, but don't exit
:w !sudo tee % | write out the current file using sudo
:wq or :x or ZZ | write (save) and quit
:q              | quit (fails if there are unsaved changes)
:q! or ZQ       | quit and throw away unsaved changes
:help keyword | open help for keyword
:o file       | open file
:saveas file  | save file as
:close        | close current pane
h             | move cursor left
j             | move cursor down
k             | move cursor up
l             | move cursor right
H             | move to top of screen
M             | move to middle of screen
L             | move to bottom of screen
r             | replace a single character
J             | join line below to the current one
cc            | change (replace) entire line
cw            | change (replace) to the start of the next word
ce            | change (replace) to the end of the next word
cb            | change (replace) to the start of the previous word
c0            | change (replace) to the start of the line
c$            | change (replace) to the end of the line
s             | delete character and substitute text
S             | delete line and substitute text (same as cc)
xp            | transpose two letters (delete and paste)
.             | repeat last command
u             | undo
Ctrl + r      | redo

yy            | yank (copy) a line
2yy           | yank (copy) 2 lines
yw            | yank (copy) the characters of the word from the cursor position to the start of the next word
y$            | yank (copy) to end of line
p             | put (paste) the clipboard after cursor
P             | put (paste) before cursor
dd            | delete (cut) a line
2dd           | delete (cut) 2 lines
dw            | delete (cut) the characters of the word from the cursor position to the start of the next word
D             | delete (cut) to the end of the line
d$            | delete (cut) to the end of the line
d^            | delete (cut) to the first non-blank character of the line
d0            | delete (cut) to the begining of the line
x             | delete (cut) character

:sp file      | open a file in a new buffer and split window
:vsp file     | open a file in a new buffer and vertically split window
Ctrl + ws     | split window
Ctrl + ww     | switch windows
Ctrl + wq     | quit a window
Ctrl + wv     | split window vertically
Ctrl + wh     | move cursor to the left window (vertical split)
Ctrl + wl     | move cursor to the right window (vertical split)
Ctrl + wj     | move cursor to the window below (horizontal split)
Ctrl + wk     | move cursor to the window above (horizontal split)

:tabnew or :tabnew file | open a file in a new tab
Ctrl + wT               | move the current split window into its own tab
gt or :tabnext or :tabn | move to the next tab
gT or :tabprev or :tabp | move to the previous tab
<number>gt              | move to tab <number>
:tabmove <number>       | move current tab to the <number>th position (indexed from 0)
:tabclose or :tabc      | close the current tab and all its windows
:tabonly or :tabo       | close all tabs except for the current one
:tabdo command          | run the command on all tabs (e.g. :tabdo q - closes all opened tabs)
