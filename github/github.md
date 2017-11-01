# git与github

## 第一步配置全局用户名

```shell
git config --global user.name ReZhangxin
git config --global user.email 1307881527@qq.com

//查询 git config user.name
```
## SSH Keys

在终端输入`ssh-keygen -t rsa -C "1307881527@qq.com"`

输入密码  zhangxin

为了保存密码不让每次执行时都输入密码 在终端输入 `ssh-agent -s` 

`ssh-add ~/.ssh/id_rsa`

打开内容复制到GitHub 验证keys

`ssh -T git@github.com`


