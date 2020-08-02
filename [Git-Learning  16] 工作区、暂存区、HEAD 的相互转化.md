#### [Git-Learning : 16] 工作区、暂存区、HEAD 的相互转化

##### 一、将暂存区恢复成HEAD（取消所有暂存）

```shell
$ git reset HEAD （-- <files> 不加文件则全部取消，加文件则取消部分）
```

##### 二、将工作区恢复成暂存区

```shell
$ git checkout  -- <files> （一定要加文件）
```