# log-cut

### 使用场景
有开发或任何非运维需要某台服务器的应用日志，这时候他们不能登录生产服务器
如果手动登录应用服务器去截取日志，效率太低

### 使用方法

* `hosts`文件中配置好对应的ftp服务器及应用服务器地址
* `log-cut.yml`中写上日志地址及截取日志时间
* 执行命令：
	```ansible-playbook log-cut.yml   --extra-vars="group=tomcat dever=zhangsan"```
