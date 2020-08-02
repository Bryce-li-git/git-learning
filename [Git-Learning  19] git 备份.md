#### [Git-Learning : 19] git 备份

一、常用的传输协议

<img src=".assets/image-20200802115539944.png" alt="image-20200802115539944" style="zoom:67%;" />

- 直观区别：哑协议传输速度不可见；智能协议传输可见
- 传输速度：智能协议比哑协议传输速度更快

二、备份的特点

<img src=".assets/image-20200802115824683.png" alt="image-20200802115824683" style="zoom:67%;" />

三、本地备份

命令：

```shell
$ git clone --bare .git_path new.git
```

