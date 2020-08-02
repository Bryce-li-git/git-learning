#### [Git-Learning : 18] git 储藏

一、储藏的意义

将当前工作区的内容存档，但不会保存暂存区的内容。

二、创建储藏

```shell
$ git stash 
```

三、恢复储藏

```shell
$ git stash apply stash_id (应用最新的储藏,不删除储藏)
$ git stash pop (应用最新的储藏，并删除)
```

四、列出所有储藏

```shell
$ git stash list
```

