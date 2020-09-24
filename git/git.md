# git 



## git初级使用

```bash
git config --global user.name "mvpbang" # 配置用户名
git config --global user.email "123456789@qq.com" # 配置邮箱
git config --global credential.helper store   # 记住密码
git config --list # 查看配置信息
```

```bash
git remote add origin "repository url" 
git remote rm origin 
git add .
git commit -m "first commit"
```



## 推送时报错

![image-20200924221558139](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200924221558139.png)

Github 禁用了TLS v1.0 and v1.1，必须更新Windows的git凭证管理器，才行。

https://github.com/Microsoft/Git-Credential-Manager-for-Windows/releases/tag/v1.14.0

点击下载安装 GCMW-1.14.0.exe ，问题就解决了。

