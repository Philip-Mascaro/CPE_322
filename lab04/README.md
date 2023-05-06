note: will add copyable commands later
'''
$ pip3 -V
$ pip3 list
$ sudo pip3 install -U setuptools
$ sudo pip3 install -U django
$ sudo pip3 install -U djangorestframework
$ sudo pip3 install -U django-filter
$ sudo pip3 install -U markdown
$ sudo pip3 install -U requests
'''
![l4s01.png](images/l4s01.png)
![l4s02.png](images/l4s02.png)
![l4s03.png](images/l4s03.png)
![l4s04.png](images/l4s04.png)
![l4s05.png](images/l4s05.png)
![l4s06.png](images/l4s06.png)
![l4s07.png](images/l4s07.png)
![l4s08.png](images/l4s08.png)


skip this: "2. Optional: Install MariaDB server and client on Raspberry Pi", move on to "3. Start Django project stevens"
```
pi@raspberrypi:~ $ django-admin startproject stevens
pi@raspberrypi:~ $ cd stevens
pi@raspberrypi:~/stevens $ ls
```
```
pi@raspberrypi:~/stevens $ python3 manage.py startapp myapp
pi@raspberrypi:~/stevens $ ls
```
```
pi@raspberrypi:~ $ sudo mysql -u root -p
```
remember "By default, Django uses SQLite"\
attempt using sqlite instead of mysql in previous command\
realize that the optional step 2 is, in fact, not optional
![l4s09.png](images/l4s09.png)

```
$ sudo apt update
$ sudo apt install mariadb-server mariadb-client
$ sudo apt install python3-mysqldb
$ sudo pip3 install -U mysqlclient
$ sudo mysql_secure_installation
Enter current password for root (enter for none): 
Change the root password? [Y/n] 
New password: PASSWORD
Re-enter new password: PASSWORD
Remove anonymous users? [Y/n] 
Disallow root login remotely? [Y/n] 
Remove test database and access to it? [Y/n] 
Reload privilege tables now? [Y/n]
```
![l4s10.png](images/l4s10.png)
![l4s11.png](images/l4s11.png)
![l4s12.png](images/l4s12.png)
![l4s13.png](images/l4s13.png)

```
pi@raspberrypi:~ $ sudo mysql -u root -p
Enter password: PASSWORD
MariaDB [(none)]> use mysql
MariaDB [mysql]> select user, host from mysql.user;
MariaDB [mysql]> create user pi@localhost identified by 'PASSWORD';
MariaDB [mysql]> show databases;
MariaDB [mysql]> create database stevens;
MariaDB [mysql]> grant all privileges on stevens.* to pi@localhost;
MariaDB [mysql]> quit
```
![l4s14.png](images/l4s14.png)
![l4s15.png](images/l4s15.png)
![l4s16.png](images/l4s16.png)

```
pi@raspberrypi:~/stevens $ cd stevens
pi@raspberrypi:~/stevens/stevens $ ls
pi@raspberrypi:~/stevens/stevens $ nano settings.py
```
```
Follow ~/iot/lesson4/stevens/settings.txt, e.g., add an asterisk to ALLOWED_HOSTS and 'myapp' to INSTALLED_APPS
The comma after 'myapp' is required
Remember to change PASSWORD for MySQL user pi
```
![l4s17.png](images/l4s17.png)
![l4s18.png](images/l4s18.png)
![l4s19.png](images/l4s19.png)
![l4s20.png](images/l4s20.png)
![l4s21.png](images/l4s21.png)


```
pi@raspberrypi:~/stevens/stevens $ cp ~/iot/lesson4/stevens/urls.py .
pi@raspberrypi:~/stevens/stevens $ cd ..
```
```
pi@raspberrypi:~/stevens $ cd myapp
pi@raspberrypi:~/stevens/myapp $ ls
pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/admin.py .
pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/models.py .
pi@raspberrypi:~/stevens/myapp $ cp ~/iot/lesson4/stevens/views.py .
```
```
pi@raspberrypi:~/stevens/myapp $ mkdir static templates
pi@raspberrypi:~/stevens/myapp $ cd templates
pi@raspberrypi:~/stevens/myapp/templates $ mkdir myapp
pi@raspberrypi:~/stevens/myapp/templates $ cd myapp
pi@raspberrypi:~/stevens/myapp/templates/myapp $ cp ~/iot/lesson4/stevens/index.html .
```
![l4s22.png](images/l4s22.png)

ghghgh
![l4s23.png](images/l4s23.png)
![l4s24.png](images/l4s24.png)
![l4s25.png](images/l4s25.png)
![l4s26.png](images/l4s26.png)
![l4s27.png](images/l4s27.png)
![l4s28.png](images/l4s28.png)
![l4s29.png](images/l4s29.png)
![l4s30.png](images/l4s30.png)
![l4s31.png](images/l4s31.png)
![l4s32.png](images/l4s32.png)
![l4s33.png](images/l4s33.png)
![l4s34.png](images/l4s34.png)
![l4s35.png](images/l4s35.png)
![l4s36.png](images/l4s36.png)
![l4s37.png](images/l4s37.png)
![l4s38.png](images/l4s38.png)
![l4s39.png](images/l4s39.png)
![l4s40.png](images/l4s40.png)
![l4s41.png](images/l4s41.png)
![l4s42.png](images/l4s42.png)
![l4s43.png](images/l4s43.png)
![l4s44.png](images/l4s44.png)
![l4s45.png](images/l4s45.png)
![l4s46.png](images/l4s46.png)
![l4s47.png](images/l4s47.png)
![l4s48.png](images/l4s48.png)
![l4s49.png](images/l4s49.png)
![l4s50.png](images/l4s50.png)
![l4s51.png](images/l4s51.png)
![l4s52.png](images/l4s52.png)
![l4s53.png](images/l4s53.png)
![l4s54.png](images/l4s54.png)
![l4s55.png](images/l4s55.png)
![l4s56.png](images/l4s56.png)
![l4s57.png](images/l4s57.png)
![l4s58.png](images/l4s58.png)
![l4s59.png](images/l4s59.png)
![l4s60.png](images/l4s60.png)
![l4s61.png](images/l4s61.png)
![l4s62.png](images/l4s62.png)
![l4s63.png](images/l4s63.png)
![l4s64.png](images/l4s64.png)


TROUBLESHOOTING STARTS HERE
![l4s65.png](images/l4s65.png)
![l4s66.png](images/l4s66.png)
![l4s67.png](images/l4s67.png)
![l4s68.png](images/l4s68.png)
![l4s69.png](images/l4s69.png)
![l4s70.png](images/l4s70.png)
![l4s71.png](images/l4s71.png)
![l4s72.png](images/l4s72.png)
![l4s73.png](images/l4s73.png)
![l4s74.png](images/l4s74.png)
![l4s75.png](images/l4s75.png)
