<<<<<<< HEAD
# MusicSpider
QQ音乐爬虫 网易云音乐爬虫 vip音乐下载 用户交互界面
![image](https://github.com/Zzjw527/MusicSpider/blob/master/p3.png)

=======
#python-播放器

##环境搭建
python3.0  MySQL数据库   mysql管理工具：Navicat for MySQL


##使用说明：
打开db_tools文件夹中的mysql1.py,修改db-》

host="xxxxxt"        本地ip 一般填localhost或127.0.0.1

port=xxxx              接口，一般为3306

user="xxx"             用户名，一般为root

passwd="xxxxxxx" 密码

db="xxxx"              数据库名字

然后再运行srart.py即可

##导入库
re                       正则表达式

json                   将字符串形式的json数据转化为字典

urilib/requests   爬虫

tkinter                图形用户界面(GUI)

pygame             连接数据库

tkinter.messagebox  提示框

##思路：
播放器/
|-- views/               界面
----
|   |-- __init__.py

|   |-- main.py          程序运行主体程序1

|   |-- main1.py         程序运行主体程序2

|   |-- disembark.py     实现登陆界面

----
|-- game/                游戏

|   |-- __init__.py

|   |-- gamemodel.py     游戏模块

|   |-- listenmusic.py   音乐播放模块

|  |-- image            图片

----

|-- db_tools/            MySQL数据库

|   |-- __init__.py

|   |-- mysql1.py        实现数据导入数据库和防止重复下载功能

----
|-- src/                 爬虫文件

|   |-- __init__.py 

|   |--qqmusic.py        爬取qq音乐

|   |--translate.py      爬取有道翻译

|   |--wangyiyun.py  爬取网易云音乐


----

|-- start.py           程序启动文件

|-- README.md           程序使用说明

|-- 优缺点.word           优缺点

----

##提示：
1、运行程序，可设置用户账号密码，数据库会记录不同用户输入记录，默认5201314，因方便观看，密码不采用**方式输出

2、下载歌曲时，如果出现程序未响应，是因为网络原因，等待1~2s即可

3、按游戏模块若未弹出图片可在game文件夹的gamemodel.py改变图片所在地址即可，因某种原因不小心删掉了游戏代码故未完成，该文件夹中有
贪吃蛇游戏SNAKE.py因并非自己所写故未添加进播放器中

4、因技术原因，要将下载记录输入数据库时无法批量下载故添加多一个批量下载按钮，即多选时无法实现立即下载按钮功能

5、当提示已下载该歌曲，会发现立即下载按钮下限，但其实还可以再次使用

6、更多优缺点可看word文档优缺点




>>>>>>> first commit
