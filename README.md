# spider-1
## ubuntu爬虫环境安装
### 工具软件
pycharm（python编写软件）\
MongoDB（数据库）\
Robmongo(查看数据库)
### 安装python和一些库
<pre>
apt-get install python3-dev build-essential libssl-dev libffi-dev libffi-dev libxml2 libxml2-dev libxslt-dev zlib1g-dev
apt-get install python3
apt-get install python3-pip
</pre>
### 安装mongodb
<pre>
apt-get install mongodb -y    安装
mongod --dbpath=/var/lib/mongodb      启动/etc/mongodb.conf
mongo    /*另开一个终端运行*/  
</pre>
### 安装redis
<pre>
apt-get install redis-server -y    
redis-cli     redis命令行模式    /etc/redis/redis.conf
redis-cli  -a  密码值    密码权限
</pre>
### 安装mysql
<pre>
apt-get  install mysql-server mysql-client
vim /etc/mysql/mysql.conf.d/mysql.cnf      修改bind-addrees 连接，使其允许远程连接
</pre>
### 多版本共存（windows 使用重命名法）
<pre>
ln -s  /use/bin/python2.7 /use/bin/python2
ln -s /use/bin/python3.5 /use/bin/python3
</pre>
### 安装写爬虫脚本需要的库(python2->pip install       python3->pip3 install)
<pre>
pip3 install requests selenium beautifulsoup4 pyquery pymysql pymongo redis flask django jupyter
</pre>
