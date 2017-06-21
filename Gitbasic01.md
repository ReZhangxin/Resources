# Git初步入门01

>git的学习

---
创建一个版本库非常简单，
首先，选择一个合适的地方，创建一个空目录：
```
$ mkdir test
$ cd test
$ pwd    //pwd命令用于显示当前目录
/Users/michael/learngit
```

第二步，通过`git init`命令把这个目录变成Git可以管理的仓库：
```
$ git init //输入命令
Initialized empty Git repository in /Users/michael/learngit/.git/
```
>把一个文件放到Git仓库只需要两步

第一步，用命令`git add`告诉Git，把文件添加到仓库：
```
$ git add readme.md
```
第二步，用命令`git commit`告诉Git，把文件提交到仓库：
```
$ git commit -m "my first git file name: readme"
[master (root-commit) cb926e7] wrote a readme file
 1 file changed, 2 insertions(+)
 create mode 100644 readme.md
```
`git commit`命令，`-m`后面输入的是本次提交的说明
为什么Git添加文件需要`add`，`commit`一共两步呢？因为`commit`可以一次提交很多文件，所以你可以多次add不同的文件，比如：
```
$ git add file1.txt
$ git add file2.txt file3.txt
$ git commit -m "add 3 files."
```
##小结
初始化一个Git仓库，使用`git init`命令。

添加文件到Git仓库，分两步：

 - 第一步，使用命令`git add` <file>，注意，可反复多次使用，添加多个文件；
 - 第二步，使用命令`git commit`，完成。

