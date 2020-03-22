# command-line environment

**看见印度老师就尼玛头大**

##  signal/ bg/ fg

python : `signal.signal(signal.SIGINT, sigint_hander)` 将SIGINT中断交给sigint_handler函数处理

example of sigint_handler:

```python
def sigint_handler(signum, time):
        print("\niv got an SIGINT signal!")
```

`^\` SIGQUIT ，similar to SIGINT, but also dumps the core

`nohup command &` run `command` without handling SIGHUP,  `&` make the cmd run in the background

`jobs` to show the background programs

`bg` to resume suspended jobs in the background `fg` to continue a job by running it in the foreground

## `tmux` manual

[more details about tmux operation](https://gist.github.com/andreyvit/2921703)

`tmux`  need to be installed ，a terminal multiplexer 

`tmux new -s <name>` to create a session names <name>

`tmux detach` or `Ctrl + b  d` to detach process with session

`tmux ls` or `mux list-session` to display all the tmux session

`tmux a` or `tmux attach` to reconnect to an existing session

`tmux a -t <name>` to reconnect to  a specific session

`tmux kill-session -t <name>`   to kill a session

`tmux kill-server` to kill all sessions

综上所述，以下是 Tmux 的最简操作流程。

> 1. 新建会话`tmux new -s my_session`。
> 2. 在 Tmux 窗口运行所需的程序。
> 3. 按下快捷键`Ctrl+b d`将会话分离。
> 4. 下次使用时，重新连接到会话`tmux a -t my_session`。

tmux pane:

> `C-b "` or `tmux split-window` 			split vertically
>
> `C-b %` or `tmux split-window -h` 	 split horizontally
>
> `C-b ArrowKeys`									to switch between panes
>
> `C-b x`		Kill the current pane

tmux window:

> `C-b c` 		create a new window
>
> `C-b &` 		kill a window
>
> `C-b 0...9` switch to window 0...9
>
> `C-b p`		previous window
>
> `C-b n`		next window
>
> `C-b l`		last (previously used) window
>
> `C-b w` 		choose window from a list
>
> `C-b ,` 		rename window
>
> 



## alias

**set in ~/.bashrc**

alias ll="ls -lahF"` set the alias

`alias sl=ls` 

`alias mv="mv -i"` replace `mv` with `mv -i` which will ask me if this command will **overwrite** an existing file 

##  zsh

[MacTalk: Why use zsh](https://zhuanlan.zhihu.com/p/19556676)

- [ ] try zsh

## dotfile

[github: dotfiles](https://github.com/search?q=dotfiles)

use **symlinks** to store all the .vimrc/.gitconfig/... in ~/dotfiles 

`ln -s <source_name> <link_name>`

## ssh

`scp`

`rsync` 

