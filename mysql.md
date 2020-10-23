### mysql的安装和配置
	安装：输入mysql，进入官网，下载社区版本的xxx.msi安装程序
	配置：找到安装路径C:\Program Files\MySQL\MySQL Server 8.0\bin，将此地址配置在系统变量的path中，确定
	测试是否安装成功：cmd管理员身份运行 mysql --version 查看安装版本
	
### mysql的启动和停止
	方法1：此电脑右键->管理->服务和应用程序->双击服务，找到mysql80(我的是mysql80),右键启动和停止
	方法2：cmd管理员身份运行 net start mysql80启动服务器  net stop mysql80停止服务器

### mysql的登录和退出
	注意：只有服务器启动之后，才能实现登录
	登录：
		方法1：在开始中找到mysql 8.0 command line client, 输入密码即可，只限于root
		方法2：cmd管理员身份运行 mysql -u root -p, 输入密码即可
	退出：
		exit 或 ctrl+c

### 查看数据库
	1.查看所有的数据库：	
	show databases;
	2.进入到指定的数据库：
	use sys;
	查看此数据库下的表格：	show tables;
	查看其它数据库有那些表：show tables from mysql;
	查看所在的数据库名：	select database();
	
	查看数据库版本：
		方法1：select version();
		方法2：exit退出sql数据库，进入到dos命令窗口，执行 mysql --version 或 mysql -V
	

