# git
基础操作
### 配置全局账户  
设置提交代码时的用户信息。
```
git config --global user.name  "您的 TGit 用户名"
git config --global user.email "您的账号 ID@git.tce.fsphere.c"
```  

### 初始化仓库
创建一个空的Git存储库或重新初始化一个已有的存储库。
```
git init
```   

### 克隆
将一个存储库复制到一个新目录中。
```
git clone [url]
```

### 添加
添加指定文件到暂存区。
```
git add [file1] [file2] ...
```  

添加指定目录到暂存区，包含子目录。
```
git add [dir]
```  

递归地添加当前工作目录中的所有文件。  
```
git add .
```  

### 删除
   
删除工作区文件，并且将这次删除放入暂存区。
```
git rm [file1] [file2] ...
```  

停止追踪指定文件，但该文件会保留在工作区。
```
git rm --cached [file]
```  

### 提交
提交暂存区到仓库区。
```
git commit -m [message]
```  

提交暂存区的指定文件到仓库区。
```
git commit [file1] [file2] ... -m [message]
```  

### 分支
列出所有本地分支。
```
git branch
```

列出所有远程分支。
```
git branch -r
```

新建一个分支，但依然停留在当前分支。
```
git branch [branchname]
```

新建一个分支，并切换到该分支。
```
git checkout -b [branch]
```

### 合并
合并指定分支到当前分支。
```
git merge [branch]
```

### 拉取
从远程仓库中获取并尝试合并到当前分支中。
```
git pull [remote] [branch]
``` 

### 推送
上传本地指定分支到远程仓库。 
```
git push [remote] [branch]
```

强行推送当前分支到远程仓库，即使有冲突。 
```
git push [remote] --force
```

推送所有分支到远程仓库。 
```
git push [remote] --all
```
