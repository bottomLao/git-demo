revert: 还原
reset: 重置
rebase
```git
# git revert
放弃某次提交, 但之前的提交日志仍会保留在git log中
```
```git
# git reset
git reset --hard
此次提交之后的修改不做任何保留，git status干净的工作区, 执行git log 后看不到了
git reset --soft
此次提交之后的修改会被退回到暂存区
```
```git
# git rebase 
当两个分支不在一条直线上，需要执行merge操作时，使用该命令操作。
git rebase -i 合并多个commit
-i 实际上就是 --interactive 的简写，在使用 git rebase -i 时，我们要在后面再添加一个参数，这个参数应该是 最新的一个想保留的 Commit
```
```git
多个commit合并
git rebase -i b45e8f9
或者
git rebase -i HEAD~3

squash：使用该 Commit，但会被合并到前一个 Commit 当中



```