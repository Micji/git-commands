### git fetch
fetches all remote branches

### git branch
shows current branch

### git branch -a
lists all branches

### git checkout path/path-file
switches to specified branch

### git checkout -b newpath/newpath-file
creates a new local branch and switches to it

### git push --set-upstream origin nPath/e-file
pushes local branch to remote repo

---

### configure basic settings and set vs.code as default editor for rebasing/merging
git config --global user.name "Your Name"  
git config --global user.email your@email.cool  
git config --global core.editor code  
git config --global merge.tool code  
  
---

## Rebasing in 10 simple steps (wait until you see number 7!)
*configure settings and tools before starting*
1. git fetch
2. git checkout master
3. git pull
4. git checkout pathTo/urBranch
5. git pull
6. git rebase master
    * get merge message
    * open code
    * resolve conflicts
    * ctrl + s to save
    * git add .
    * git rebase --continue
    * **REPEAT FOR EVERY COMMIT**
7. git pull
8. merge commit message
9. save & quit
10. git push