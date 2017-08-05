# 4．**Ionic安装与使用**

****

### 一、Windows系统

#### 1、 ionic安装 


* 安装ionic

   `npm install -g ionic`

* 安装bower包管理器

   `npm install -g bower`

    <u>至此，Ionic相关组件安装完毕</u>

####2、**ionic使用**


* 创建ionic项目

  `ionic start xxxx blank` （当中XXX即项目名）

* 在确保bower包管理器安装成功的情况下并在项目目录下安装ngCordova

  `bower install ngCordova`

* 指定到当前项目目录

  `cd XXXX`（若未指向当前项目目录，需要指定项目目录中打开git终端） 

* 在platform中添加并创建一个android目录

  `ionic platform add android`

  `ionic build android`

* 运行ionic项目

  `ionic run android` 

****

### 二、MAC OS X系统

####1、ionic安装

* 安装ionic（sudo获取权限）

  `sudo npm install -g ionic`

* 安装bower包管理器    
   `sudo npm install -g bower`

    <u>至此，MAC OS X下Ionic相关组件安装完毕</u>

####2、ionic的使用

* 创建ionic项目

  `ionic start xxxx blank` （当中XXX即项目名）

* 在确保bower包管理器安装成功的情况下并在项目目录下安装ngCordova库

  `bower install ngCordova`

* 指定到当前项目目录

  `cd XXXX`（若未指向当前项目目录，需要指定项目目录中打开git终端）

* 在platform中添加并创建一个android目录

  `ionic platform add ios`

  `ionic build ios`

* 运行ionic项目

  `ionic run ios` 