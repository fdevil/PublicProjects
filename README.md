# 这是一个公共仓库


## 简介
<<<<<<< HEAD
这一次链接成功，学习资料来自[Git 详解 - 简书](https://www.jianshu.com/p/382abb427ca9 "Git 详解 - 简书")
今天真的很搞笑
=======
这一次链接成功，学习资料来自[Git 详解 - 简书](https://www.jianshu.com/p/382abb427ca9 "Git 详解 - 简书")。
这一次成功上传和下载，我很高兴。
>>>>>>> 1a458e434eeb763bdf96380a11f7ea0b060b2a74

这一次 首先在远端服务器修改README.md文件
添加“这一次成功上传和下载，我很高兴。”

同时在本地修改README.md文件
添加“今天真的很搞笑”


在执行git pull origin master后 Please commit your changes or stash them before you merge.在合并之前，请提交更改或存储更改。
其实就是要将远端和本地合并必须使本地的文件已经提交执行 git commit -m "".


    
Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master)
$ git pull origin master
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 702 bytes | 8.00 KiB/s, done.
From https://github.com/fdevil/PublicProjects
 * branch            master     -> FETCH_HEAD
   3473087..1a458e4  master     -> origin/master
error: Your local changes to the following files would be overwritten by merge:
        README.md
Please commit your changes or stash them before you merge.
Aborting
Updating 3473087..1a458e4

Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master)
$ git add README.md

Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master)
$ git pull origin master
From https://github.com/fdevil/PublicProjects
 * branch            master     -> FETCH_HEAD
error: Your local changes to the following files would be overwritten by merge:
        README.md
Please commit your changes or stash them before you merge.
Aborting
Updating 3473087..1a458e4

Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master)
$ git status
On branch master
Your branch is behind 'origin/master' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master)
$ git commit -m "update"
[master 36885a0] update
 1 file changed, 1 insertion(+)

Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master)
$ git pull origin master
From https://github.com/fdevil/PublicProjects
 * branch            master     -> FETCH_HEAD
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.

Administrator@DEEP-2020SPOHKD MINGW64 /e/GitProjects/PublicProjects (master|MERGING)


## 用法
