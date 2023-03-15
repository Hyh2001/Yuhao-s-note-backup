存储库通常用于组织单个项目。存储库包含**项目所需的任何内容以及这些内容的修改历史**。通常，存储库包括一个 [[README]] 文件。
存储库分为
1. [[Git local repository]]
2. [[Git remote repository]] 

# Git repository commands 
## 创建一个新的 repository 
git init initializes a brand new Git repository and begins **tracking** an existing directory. It adds a **hidden subfolder** within the existing directory that houses the internal data structure required for version control.
```shell 
git init # 在一个文件夹中git init 会创建一个新的文件夹
```

## 复刻远程 repository
git clone creates a **local copy** of a project that already exists remotely. The clone includes all the project's files, history, and [[Git branch]].
```shell
git clone /path/to/repository # 这个命令会复刻本地的一个仓库
git clone username@host:/path/to/repository #复刻远端服务器上的仓库
```

## 





https://www.runoob.com/manual/git-guide/
https://docs.github.com/en/get-started/using-git/about-git