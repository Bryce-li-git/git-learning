#### [Git-Learning : 15] git diff 比较差异

##### 一、比较暂存区和HEAD

```shell
$ git diff --cached
```

![image-20200731111325848](.assets/image-20200731111325848.png)

##### 二、比较工作区和暂存区

```shell
$ git diff 
```

![image-20200731111710789](.assets/image-20200731111710789.png)

##### 三、比较两个commit或branch

```shell
$ git diff commit01_id commit02_id -- <files>
$ git diff branch01_id branch02_id -- <files>
```

