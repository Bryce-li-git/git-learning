#### [Git-Learning : 12] git branch 管理

##### 一、切换分支，将HEAD指向另一个branch或者commit

```shell
$ git checkout aim_branch
$ git checkout aim_commit (变为分离头指针状态，没有工作在任何一个branch上)
```

##### 二、创建新分支

```shell
$ git branch new_branch commit_hashcode  (分离头指针后常用)
$ git checkout -b new_branch base_branch 
                                       (基于某一个分支而新建，并切换到新分支)
```

##### 三、查看分支信息

```shell
$ git branch (只能在仓库的工作目录下使用)
```

##### 四、删除旧分支

```shell
$ git branch -d old_branch
$ git branch -D old_branch (强制删除)
```

##### 五、改变分支指向
```shell
$ git branch -f target_branch where
$ git rebase branch1 branch2 （在同一条分支上可以将branch2指向改为branch1）
```

##### 六、整理分支

```shell
$ git rebase branch1 branch2 (将branch2的所有不同的commit加到branch1上)
```

##### 七、相对引用

相对引用

- 使用 `^` 向上移动 1 个提交记录，HEAD^
- 使用 `~<num>` 向上移动多个提交记录，如 `~3`，HEAD~3