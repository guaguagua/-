###  1. git: Permission denied (publickey)
- 问题现象  
```
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.
Please make sure you have the correct access rights
and the repository exists.
```

- 环境  
  已经在linux生成key,并配置到github,而且正常使用过  
  
- 解决方式  
  - [参考](https://www.cnblogs.com/wmr95/p/7852832.html)  
  - `ssh-agent -s`  
  - `` eval `ssh-agent -s` ``  
  - `ssh-add ~/.ssh/id_rsa`  
