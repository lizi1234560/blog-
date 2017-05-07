基于 django 1.10 和 Python 3.5 的 django 博客开发入门教程，带领你从零开始一步步开发属于自己的个人博客，让你以最快的速度掌握 django 开发的技巧。

## 项目演示地址

http://demo.zmrenwu.com/

## 项目教程

本项目配有完整的教程说明，教程阅读地址：[django 博客开发入门教程](http://zmrenwu.com/category/django-blog-tutorial/)。

每篇教程的代码都位于项目相应的分支中，点击上方的 **Branch** 按钮可以查看到，例如分支 Step1_build-development-environment 对应第 2 篇教程 [2. 搭建开发环境](http://zmrenwu.com/post/3/)。

master 主分支是整个项目的完整代码。

## 在本地运行项目

1. 克隆项目到本地

   打开命令行，进入到保存项目的文件夹，输入如下命令：

   ```
   git clone https://github.com/zmrenwu/django-blog-tutorial.git
   ```

2. 创建并激活虚拟环境

   在命令行进入到保存虚拟环境的文件夹，输入如下命令创建并激活虚拟环境：

   ```
   virtualenv blogproject_env

   # windows
   blogproject_env\Scripts\activate

   # linux
   source blogproject_env/bin/activate
   ```

   关于如何使用虚拟环境，参阅：[2. 搭建开发环境](http://zmrenwu.com/post/3/)的 Virtualenv 部分。

   如果不想使用虚拟环境，可以跳过这一步。

3. 安装项目依赖

   如果使用了虚拟环境，确保激活并进入了虚拟环境，在命令行进入项目所在的 django-blog-tutorial 文件夹，运行如下命令：

   ```
   pip install -r requirements.txt
   ```

4. 迁移数据库

   在上一步所在的位置运行如下命令迁移数据库：

   ```
   python manage.py migrate
   ```

5. 创建后台管理员账户

   在上一步所在的位置运行如下命令创建后台管理员账户

   ```
   python manage.py createsuperuser
   ```

   具体请参阅：[8. 在 django admin 后台发布我们的文章](http://zmrenwu.com/post/9/)

6. 运行开发服务器

   在上一步所在的位置运行如下命令开启开发服务器：

   ```
   python manage.py runserver
   ```

   在浏览器输入：127.0.0.1:8000

7. 进入后台发布文章

   在浏览器输入：127.0.0.1:8000/admin

   使用第 5 步创建的后台管理员账户登录

   具体请参阅：[8. 在 django admin 后台发布我们的文章](http://zmrenwu.com/post/9/)

## 交流讨论和继续学习 django

这里汇聚了大量经验丰富的 django 开发者，遇到问题随时请教，以及获取更多的 django 学习资料。

- django 学习小组 QQ 群：561422498
- django 学习交流论坛：[Python 中文社](http://pythonzh.cn/)
- django 学习小组邮件列表：django_study@groups.163.com
- django 博客，更多 django 开发文章和教程：[追梦人物的博客](http://zmrenwu.com/)
- [django 入门学习规划与资料推荐](http://zmrenwu.com/post/15/)
