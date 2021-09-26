# 1、服务器的SSL证书没有经过第三方机构的签署

+ 报错形式
  + fatal: unable to access 'https://github.com/lulong9527/Git-.git/': OpenSSL SSL_read: Connection was reset, errno 10054

* 解决方法
  * 确定登录GitHub后，在多次尝试操作推送等操作
  * git config --global http.sslVerify “false”

+ 参考文档: <https://www.cnblogs.com/jfen625/p/12995408.html>

# 2、Git branch 出现"HEAD detached at head xxxxx"

前提：删除本地分支出现HEAD detached at head ，执行以下步骤

+ git branch <your-branch-name> xxxxx           # 给 xxxxx 起个 branch 名

+ git checkout master                                        # Head 指到 master，当然可以是其它的branch

+ git merge <your-branch-name>                      # 合并到当前 主干branch

+ git branch -d <your-branch-name>                 # 删除临时 branch