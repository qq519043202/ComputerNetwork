## Re:从零开始的Ubuntu配置

### qcloud
- ssh ubuntu@123.206.196.117

### LAMP
- [某博客](http://www.linuxeden.com/html/softuse/20140610/152522.html)
- 他说用root就root吧。。
- 先更新一波源


- 发现无法 sudo service apache2 restart .
- 在 /etc/apache2/apache2.conf 里加一句 ServerName localhost:80
- phpmyadmin在/usr/share/phpmyadmin目录，所以就用命令：sudo ln -s /usr/share/phpmyadmin /var/www/html 建立连接。


- sudo service mysql []
- sudo service apache2 []

(13)Permission denied: AH00072: make_sock: could not bind to address [::]:80
(13)Permission denied: AH00072: make_sock: could not bind to address 0.0.0.0:80
这个错是因为没用root权限。。


- sudo apt-get install apache2-dev //装apxs
- make是出现问题。。百度google。
- sudo apt-get install python-dev