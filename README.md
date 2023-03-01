# 项目介绍:个人简易云盘,基于Django框架
### 环境:python 3.7,Django 2.1.7,mysql 5.7,pymysql 0.9.3, Bootstrap 3.3.7,jQuery v3.3.1
## 项目预览:
![avatar](https://github.com/swpu-cxm/cloud/blob/master/cloud.png)
## 基本功能:
+ 1.用户注册,登录,用户数据存放在mysql中,为Django的user_auth表
+ 2.创建用户目录,目录名为用户名,并在用户主下面建立五个分类子目录
用来存放不同分类的文件
+ 3.用户登录后可查看自己的文件,可以实现文件的上传,在线预览,下载,删除
+ 4.页面功能:
  + 1右侧链接栏为分类区,通过ajax刷新左侧文件显示区表格
  + 2表格上方为上传按钮,和搜索栏,可以进行分类搜索,并通过ajax动态刷新表格内容
## 更新功能:
  + 1.重构文件存储目录及文件存储数据模型
  + 1.上传文件进度条
  + 2.添加文件夹功能,支持创建,修改,删除文件夹
  + 3.支持文件夹,文件重命名
  + 4.加了一些好看的图标...
## 如何使用:
### 1. 安装虚拟环境
    git clone https://github.com/swpu-cxm/cloud.git

    cd cloud  
    
    pipenv install --dev  
  
    pipenv shell  
  
### 2.  在settings.py中配置数据库信息,调试时请设置DEBUG=True,然后建立据库模型

    python manage.py makemigrations  
    python manage.py migrate  
  
### 3.  启动服务  
    python manage.py runserver 127.0.0.1:8000  

### 4.测试服务是否启动  

#### 浏览器访问127.0.0.1:8000,页面跳转至登录页面,测试注册,登录,上传文件,分类文件,搜索文件,删除文件等功能

















