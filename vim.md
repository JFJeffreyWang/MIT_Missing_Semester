# vim tutorial

[toc]

## keys



[vim tutorail](https://www.runoob.com/w3cnote/all-vim-cheatsheat.htm)

`hjkl` for moving

`w b` for moving a word

`0 $` for move to the start or end of the line

`gg G` for moving to the the end or start of the file

`L M H` for Low Middle High of the window

 `T t F f` find characters in line

`O o` to adding a new line

`Y y` to copy

`P p` to paste

**`;` replay `T t F f`!!!!**

`u` undo

`Ctrl + R` redo

`4j` to do `j` for 4 times

`%` to switch between l/r brackets live `[`&^&*^`]` or `(`&^*&&`)`

`di[`  or `ci[` to delete/change the contents **inside** a `[ ]` bracket

`:help object-select` for the details of eg. `di[` or `d4w`

`/` or `?` to search and `n`or`N` to switch





![](C:\Users\JeffreyWang\OneDrive\wjf_document\documents\MIT_missing\vim.assets\vi-vim-cheat-sheet-sch1.gif)

 ![classic](C:\Users\JeffreyWang\OneDrive\wjf_document\documents\MIT_missing\vim.assets\classic1.gif)

## settings

`set number` display line numbers

`set ignorecase` 设置默认进行大小写不敏感查找

`set smartcase` 如果有一个大写字母，则切换到大小写敏感查找

`set incsearch` 可以在敲键的同时搜索，按下回车把移动光标移动到匹配的词； 按下 Esc 取消搜索。

`set wrapscan` 用来设置到文件尾部后是否重新从文件头开始搜索。

`set relativenumber` to set the line numbers to relative mode **very useful**



## windows

`:split/sp/vsp filepath` open another file

or `vim -o file1 file2`

`ctrl + w + j/k` jump over windows

`:res(ize) 5` `res+5` `res -10`  adjust window size

`:vertical res 5` vertically



- [ ] todo: 尝试vundle 和 pathogen来安装Conque Shell 失败了

  虽然显示Conque Shell安装成功，但是无法使用



