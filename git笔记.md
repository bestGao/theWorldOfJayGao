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
