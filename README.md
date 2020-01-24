# Rabbitmq
Mac 中的rabbitmq的安装与部署
安装brew,在命令窗口执行:/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" 
安装过程中提示文件夹不存在,需要按回车新建,接着输入密码即可,下载较慢,需等待下

安装完毕后执行brew update  更新brew

1)brew install rabbitmq

注意： rabbitmq的安装目录： /usr/local/Cellar/rabbitmq/3.8.2

2)启动:进入到/usr/local/Cellar/rabbitmq/3.8.2目录执行:

sbin/rabbitmq-server

ps:任意目录启动

          /usr/local/Cellar/rabbitmq/3.8.2/sbin/rabbitmq-server

RabbitMQ 启动插件
待RabbitMQ 的启动完毕之后，另起终端进入

cd /usr/local/Cellar/rabbitmq/3.8.2/sbin

sudo ./rabbitmq-plugins enable rabbitmq_management（执行一次以后不用再次执行）

登陆管理界面

浏览器输入：http://localhost:15672/

账号密码初始默认都为guest,登录后可新建一个账号密码进行管理
