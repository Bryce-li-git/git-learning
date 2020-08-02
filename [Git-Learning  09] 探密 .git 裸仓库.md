#### [Git-learning : 10] 探密 .git 裸仓库

##### 一、.git 的 文件树

```shell
.git/
├── branches
├── COMMIT_EDITMSG
├── config  (当前仓库的配置信息（local config）)
├── description
├── gitk.cache 
├── HEAD    (头指针指向当前的工作分支，保存一个ref指向refs/heads/中的某一个分支)
├── hooks
│   ├── applypatch-msg.sample
│   ├── commit-msg.sample
│   ├── fsmonitor-watchman.sample
│   ├── post-update.sample
│   ├── pre-applypatch.sample
│   ├── pre-commit.sample
│   ├── pre-merge-commit.sample
│   ├── prepare-commit-msg.sample
│   ├── pre-push.sample
│   ├── pre-rebase.sample
│   ├── pre-receive.sample
│   └── update.sample
├── index
├── info
│   └── exclude
├── logs   (版本日志信息)
│   ├── HEAD
│   └── refs
│       └── heads
│           └── master
├── objects      (object对象信息，包含commit、tree、blob)
│   ├── 15  
│   │	|   (哈希码标识对象并保存信息)
│   │   └── 64449840ce2957a90e03a24bd252045ca9998b 
│   ├── fd  (这里要将文件夹名字加子文件名字相加得到哈希值)
│   │   └── ba277feecfd772573256616741f454f2948be6
│   ├── info
│   └── pack
└── refs
    ├── heads      (分支信息，即一个独立的开发空间,指向一个commit)
    │   └── master
    └── tags       (标签（里程碑）信息,指向一个commit)
     	└── js01
```

PS:查看Object文件的命令

```shell
$ find .git/objects -type f
```

