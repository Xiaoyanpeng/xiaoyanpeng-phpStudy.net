```
下载phpstudy,安装时注意安装位置  项目拷贝到www的文件夹中
```

```
右键 phpMyAdmin 帐号密码都是root
```

```
右键 phpStudy设置 80端口检测 （环境端口检测）
```

```
右键 MySQL设置 设置密码 1234 快速创建数据库 study
```

```
右键 站点域名管理 网站域名 www.xyp.com  网站目录 安装位置/www/项目名 新增保存
```
```
右键 打开hosts 尾部添加 127.0.0.1  www.xyp.com
```
```
启动运行 在浏览器输入 www.xyp.com 即可
```
```
配置两个站点
```
```
安装路径的位置 phpStudy\Apache\conf 点击vhosts.conf
```

```
<VirtualHost *:80>
    DocumentRoot "D:\WWW\stourwebcms5.0"
    ServerName www.xyp.com
    ServerAlias phpStudy.net
  <Directory "D:\WWW\stourwebcms5.0">
      Options FollowSymLinks ExecCGI
      AllowOverride All
      Order allow,deny
      Allow from all
      Require all granted
  </Directory>
</VirtualHost>
//////下面一段是复制修改的
<VirtualHost *:80>
    DocumentRoot "C:\Users\xiao1_000\Desktop\55"
    ServerName www.xyp1.com
    #ServerAlias phpStudy.net
  <Directory "C:\Users\xiao1_000\Desktop\55">
      Options FollowSymLinks ExecCGI
      AllowOverride All
      Order allow,deny
      Allow from all
      Require all granted
  </Directory>
</VirtualHost>
```

```
右键 打开hosts 尾部添加的 127.0.0.1  www.xyp.com www.xyp1.com
```








