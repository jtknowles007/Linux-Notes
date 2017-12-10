# VIM Notes

## 11/27/2017

* :wq and ZZ do the same thing.  Save file and exit VIM.
* v enters view mode, can then use cursor to select text.
* yy will copy (or yank) text for use elsewhere
* Esc to command mode and enter :e path/to/file to open another file that you want to paste to
* p to paste after cursor, P to paste before cursor

## 11/29/2017

* Vim 101: A Beginner's Guide to Vim
    + https://www.linux.com/learn/vim-101-beginners-guide-vim
* Moving around the file - one character/line at a time
    + h moves one character LEFT
    + j moves one line UP
    + k moves one line DOWN
    + l moves one character RIGHT
* Moving around the file - word level
    + w moves forward one word at a time
    + b moves backward one word at a time
* Moving around the file - line level
    + o moves the cursor to the beginning of the line
    + $ moves the cursor to the end of the line
*  Moving around the file - file level
    + gg moves to the beginning of the file
    + G moves to the end of the file
    + `. moves to the last edit point
* Preface the movement commands with a number will execute that command n times
    + 5h moves the cursor 5 characters left
    + 3w moves the cursor 3 words forward
    + etc.

