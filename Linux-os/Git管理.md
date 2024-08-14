# Git管理

1.创建新分支

```shell
git checkout -b 新分支名 master
```



2.查看分支

```shell
git branch -vv
```



3.提交

```shell
git push --set-upstream origin modbus-zjs		# 在远程上创建并关联该新分支
```



4.gitee上创建MR，合并分支



5.切回master分支，本地同步远程

```shell
git switch master
git pull -r
```



6.新分支同步master

```shell
git switch 新分支
git rebase -r   #等同于git merge
git push -f
```

