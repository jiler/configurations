### 安装  
1. 首先下载解压版mysql5.7,并解压  
2. 打开目录，复制my-default.ini，然后改为my.ini，编辑该文件，添加
basedir = D:\\install\\mysql  
datadir = D:\\install\\mysql\\data  
具体路径自己修改，然后保存。  
3. 打开bin目录，在此处打开cmd，执行  
D:\install\mysql\bin>mysqld  --initialize-insecure  
初始化mysql.会发现多了data目录及data下的文件  
4. 启动mysql。  
在bin目录下(添加path值;d:\install\mysql\bin)，执行D:\install\mysql\bin>mysqld --console  
注意以管理员权限来执行。  
5. 之后重新开一个界面，连接mysql并修改密码  
>mysql-uroot  
Welcome to theMySQL...........  
.............  
mysql>set password=password('root');  
Query OK,0  
rows affected,1 warning(0.00 sec)  

win版的mysql，不会生成随便密码，只需要要安装时初始化就行了。  
如果是已经安装好的mysql忘了密码，可以先备份data文件夹，然后删除data文件夹，再执行3、4、5步即可。  

###增加新用户并授权  
GRANT ALL PRIVILEGES ON *.* TO 'dds'@'%' IDENTIFIED BY 'dds' WITH GRANT OPTION  
