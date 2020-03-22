# version control

[MIT: Missing Semester_Lectrue6: version control](https://missing.csail.mit.edu/2020/version-control/)

![git](git.assets/git.png)

## basic operation

`git init`

`git status`

`git add <file>`

`git commit `

`git cat-file -p 3b18e512dba79e4c8300dd08aeb37f8e728b8dad` cat-file by hash 

`git log --all --graph --decorate` show the commit history by **graph**

> `--oneline` show compact graph

`git checkout <hash/name>` switch HEAD node to <hash>

`git checkout -f <hash/name>` switch by force

`git checkout <filename>` replace \<filename\> with itself in HEAD node

`git diff (<hash/HEAD/master/...>)? <filename>`  compute the diff from `<hash>`  to **now**

`git diff <hash1> <hash2> <filename>` compute the diff from \<hash\> to  \<hash2\>



## branch

`git branch` or `git branch -vv`(for more information) to display the current branch

`git branch <name>` to create new branch

> `git checkout -b <name>`  same as `git branch <name>; git checkout <name>`

`git checkout <name>` to switch the HEAD node to \<name\> branch

`git merge <hash/name>` to merge HEAD with \<name\>

 

## remote

`git remote add <name> <url>`  like this: `git remote origin ../remote`

`git push <remote_name> <local_branch>:<remote_branch>` like this: `git push origin HEAD:master` 

`git branch --set-upstream-to=origin/master` to set 'local branch' to track remote branch 'master'

when the above setting is completed

`git push` or `git push origin` also works 

`git fetch` or `git fetch origin`to update repository by retrieving specific remote branch

`git pull` equals to  ` git fetch; git merge origin/master` 

`git clone <url> ` to clone the whole version history

- [ ] `git clone --depth 1 ` It should only clone the latest snapshot, but the measurement is useless, **WHY?**

## Some other things

`.gitignore` file

```
.DS_Store
*.o
```



[Pro Git](https://git-scm.com/book/en/v2) is **highly recommended reading**. Going through Chapters 1–5 should teach you most of what you need to use Git proficiently, now that you understand the data model. The later chapters have some interesting, advanced material.



 **test**
