# git与github

## 第一步配置全局用户名

```shell
git config --global user.name ReZhangxin / railgunxin
git config --global user.email 1307881527@qq.com

//查询 git config user.name
```
## 第二步添加：`SSH Keys`

- 在终端输入`ssh-keygen -t rsa -C "1307881527@qq.com"` 一路回车密码空就行
- 然后在`github`中添加秘钥，在桌面的`Administrator`中找到`.ssh`文件夹中的`id_rsa.pub` 中的秘钥添加到`github`中的`SSH Keys`链接
- 为了保存密码不让每次执行时都输入密码 在终端输入
```
git config --global credential.helper store
```
- 验证：$ ssh -T git@github.com /ssh -T git@git.coding.net
成功提示Hi ReZhangxin! You've successfully authenticated, but GitHub does not provide shell access.
（成功的钥匙图标是绿的不是黑的）

## 第三步：首次puh的时候要写默认的`origin master`

```
git push origin master
```
