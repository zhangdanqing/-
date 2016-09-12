#services-start
####在zsh的基础上，设置一键开启所有服务

####把以下代码复制到.zshrc里面，最下面即可。

```
alias php70.start='sudo brew services start php70'
alias php70.stop='sudo brew services stop php70'
alias php70.restart='php70.stop && php70.start'

alias php56.start='sudo brew services start php56'
alias php56.stop='sudo brew services stop php56'
alias php56.restart='php56.stop && php56.start'


alias nginx.start='sudo brew services start nginx'
alias nginx.stop='sudo brew services stop nginx'
alias nginx.restart='nginx.stop && nginx.start'

alias mysql.start='sudo brew services start mysql'
alias mysql.stop='sudo brew services stop mysql'
alias mysql.restart='mysql.stop && mysql.start'

alias nginx.start='sudo brew services start nginx'
alias nginx.stop='sudo brew services stop nginx'
alias nginx.restart='nginx.stop && nginx.start'

alias services.start='mysql.start && nginx.start && php56.start'
alias services.restart='mysql.restart && nginx.restart && php56.restart'

```
####保存退出之后执行source .zshrc，重新执行刚修改的文件，使之立即生效，而不必注销并重新登录。

##使用
命令：

services.restart  重启

services.start	 启动
