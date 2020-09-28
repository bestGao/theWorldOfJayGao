## 常用git命令

- 刷新远程分支  

```
git remote update origin --prune
```

- 删除master以外本地分支 
```
git branch | grep -v "master" | xargs git branch -D
```

- 新电脑新增GitHub权限：
```
  $ ssh-keygen -t rsa -b 4096 -C "your_email@example.com" // 生成ssh
  ```
  
- 获取最新的一条commit message
``` sh
git log -1 --pretty=%B
```
- git删除一或多条已经push的commit
``` bash
git reset --hard HEAD~number
修改之后 git push --force
```
- git修改最近一次push的commit
``` bash 
git add .
git commit --amend --no-edit
```
