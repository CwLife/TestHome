\[TOC\]

# Git 命令操作

## 场景

### 从远程克隆仓库并提交:

```shell
$ cd /Users/Alfred/Desktop/book 
$ git clone https://git.oschina.net/alfred03/book-axyz.git   # 克隆

$ cd book-axyz 
$ git status    # 查看文件状态
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

    README.md
    SUMMARY.md
    _book/
    a/
    b/
    c.md

nothing added to commit but untracked files present (use "git add" to track)

$ git add .  # 添加所有文件
$ git commit -m 'first commit'   # 提交
$ git push -u origin master   # 推送至远程仓库
```



