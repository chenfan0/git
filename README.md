# git

## 合并分支
- 可以通过`merge`， `git merge b1`  合并b1分支到当前分支
- 可以通过 `rebase`, 
  - `git checkout b1` 切换到要被合并的分支 
  - `git rebase master` 变基到master分支，也就是要合并的分支
  - `git checkout master`  切换到master分支
  - `git merge b1`  合并b1分支

如果遇到合并冲突时，先处理好冲突。然后add文件，然后在执行`git rebase --continue`即可
## pull，push
- 在push之前，需要先pull最新的远程分支的代码 `git pull origin main --rebase`
- 如果有冲突产生，需要先进行冲突解决。然后进行add，`git rebase --continue`
- 最后在进行push操作