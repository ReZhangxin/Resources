## 我的github
> 总的来说就是先要有一个仓库还得要SSH

## 第一步要先clone你的仓库地址比如说一个Html仓库
> git clone 地址

## git pull
## git add .
## git commit -m"描述"
## git push
> 生成秘钥
```
$ ssh-keygen -t rsa -C "1307881527@qq.com"
```

# SSH Keys
> 在终端输入`ssh-keygen -t rsa -C "1307881527@qq.com"`<br>
输入密码  zhangxin<br>
为了保存密码不让每次执行时都输入密码 在终端输入 `ssh-agent -s` <br>
`ssh-add ~/.ssh/id_rsa`<br>
打开内容复制到GitHub 验证keys
`ssh -T git@github.com`


