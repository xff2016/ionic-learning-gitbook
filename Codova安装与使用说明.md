
# 2．**Codova安装与使用说明**
****
### 一、iOS 安装

​     打开OS X操作系统终端（类似于Windows操作系统命令提示符窗口）通过如下方法以unix命令的方式进行安装
####1、Cordova安装

* 安装Homebrew套件管理器，具体安装过程详见

​      [http://brew.sh/index_zh-cn.html](http://brew.sh/index_zh-cn.html)

* 赋予root权限

  `sudo chown root:wheel /usr/local/bin/brew`

* 安装git包管理器（跟homebrew两个缺一不可）

    `sudo brew install git`

* 安装node

   `sudo brew install node`

* 安装Cordova

  `sudo npm install –g cordova`

* 安装ios-sim

ios-sim是一个在Mac OS X上执行的开源软件，目的是让图像设计师和管理人员等非开发者，也能将原本编译好给iOS的程式，放在iOS模拟器上执行。

      `sudo npm install -g ios-sim`

* 安装ios-deploy

     `sudo npm install –g ios-deploy

    <u>至此，Mac OS X下整个cordova安装完毕</u>



####2、创建一个Cordova项目（也是通过终端命令的方式创建）

* 创建一个名为HelloWorld的项目

​      ` cordova create hello com.example.hello HelloWorld`

​       hello ---根文件夹名字

​       com.example.hello ----项目包名

​       HelloWorld------项目名

*  指定到当前项目目录

   `cd hello`

*  在platform中添加并创建一个IOS目录

   `cordova platform add ios`

   `cordova build`

 4 运行该Cordova 项目

	`cordova run ios`



###二、安卓应用开发

目前，一般 安卓应用在Windows操作系统上开发的较多，下面介绍windows系统下cordova的安装与使用

前注：

* JDK安装，配置环境变量（需要jdk7.0以上）

* Android SDK安装，配置

####1、cordova安装

* 安装git（分布式版本控制系统）

[http://git-scm.com/download](http://git-scm.com/download)

![img](Img\wps32C7.tmp.jpg) 

选择Window版本进行安装

安装成功之后即可打开如下图所示的命令行窗口

![img](Img\wps32C8.tmp.jpg) 

* 安装nodejs 

[https://nodejs.org/en/download/](https://nodejs.org/en/download/)

![img](Img\wps32D9.tmp.jpg) 

下载windows版本进行安装

* 安装cordova

	`sudo npm install –g cordova`注意：此处使用国内的npm镜像

	`$ npm config --global set registry http://registry.cnpmjs.org`

 

安装成功之后按照以下网页上的安装步骤检查或安装

[http://www.aichengxu.com/view/44135](http://www.aichengxu.com/view/44135)

安装ant,具体安装步骤可按照以下网址进行操作

[http://www.androiddevtools.cn/](http://www.androiddevtools.cn/)

​      <ul>至此windows下Cordova安装完毕</ul>

#### 2、创建一个Cordova项目（通过git终端上的方式创建）

* 创建一个名为HelloWorld的项目

​      	`cordova create hello com.example.hello HelloWorld`

​      hello ---根文件夹名字

​      com.example.hello ----项目包名

​      HelloWorld------项目名

* 指定到当前项目目录

  	`cd hello`

* 在platform中添加并创建一个IOS目录

  	`cordova platform add android`

	`cordova build`（直接下载gradle太慢，最好手动下载）

SL：手动下载gradle，地址是（http://services.gradle.org/distributions/gradle-2.2.1-all.zip），然后把它放到路径（C:\Users\nxy\.gradle\wrapper\dists\gradle-2.2.1-all\2m8005s69iu8v0oiejfej094b）

SL：下载过程当中，会下载很多jar包，如果下载不下来，可以输入链接，手动下载，放到带有ivy.xml的文件路径中。

* 运行该Cordova 项目

	`cordova run android`

​    PS:windos下第一次创建项目时可能会下载库文件，可能会下载失败，根据错误提示需手动安装gradle
