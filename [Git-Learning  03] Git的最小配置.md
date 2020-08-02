### [Git-Learning : 03] Git的最小配置

#### 一、最小配置

 在使用git之前，需要的最小配置为：配置user.name和user.email.

```shell
$ git config --global user.name 'your_name'
$ git config --global user.email 'your_email'
```

#### 二、config 的三个作用域

```shell
$ git config --local            (默认为local，local只对某个仓库有效)
$ git config --global             (global对当前用户所有的仓库有效)
$ git config --system             (system对系统所有登录的用户有效)
```

#### 三、显示 config 的配置，加 --list

```shell
$ git config --list --local
$ git config --list --global
$ git config --list --system
```

