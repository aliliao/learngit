
# Git 常用命令

---

[TOC]

## 撤销

1. 将当前提交撤销，重置到上一次提交。撤销提交的改动保留在工作区中。`git reset [--soft | --mixed | --hard] HEAD^`

   软 --soft，中 ---mixed，硬 --hard 对应着三种回滚的程度，程度越硬，回滚的越“狠”: 

   1. `--soft` 已 add，但尚未 commit 
   2. `--mixed`（git reset 的默认设定，可以省略不写），文件会回退到未 add（未暂存）的状态 
   3. `--hard` 硬核，彻底，会彻底返回到回退前的版本状态，了无痕迹

2. 如果我们希望彻底丢掉本地修改但是又不希望更改branch所指向的commit，则执行`git reset --hard = git reset --hard HEAD`

3. [如何撤销 Git 操作？](http://www.ruanyifeng.com/blog/2019/12/git-undo.html)



参考文章：

- [常用 Git 命令清单](https://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html)