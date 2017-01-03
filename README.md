
React Native安装环境，这里的准备工作，主要分为如下几点：
   安装jdk，配置jdk的环境变量
   配置android开发环境，配置sdk的环境，这里的sdk必须有23版本
   安装genymotion，当然这里也可以使用真机调试
   安装git
   安装node.js 并配置环境变量 https://nodejs.org/en/
   react native环境搭建

1.上面的准备工作相对来说比较简单，这里我就不一一演示了，需要的朋友可以自行google，
下面正式开始搭建React native开发环境。这里，我在e盘下创建一个reactnative目录，
用来存放创建的工程，进入该目录，执行如下命令：

$ npm install -g react-native-cli
$ react-native init firstProject


2.编译android应用  至此，firstProject工程已经创建好了，进入该工程目录，执行如下命令，运行该工程：
react-native run-android

3.需要注意的是，在运行该命令的之前必须打开模拟器，或者连上真机调试。千万切记：在正式运之前，最好另外打开一个窗口，
还要通过react-native start来开启服务
服务开启完成，可以先查看下该条服务是否可用，打开谷歌浏览器，按照提示输入如下链接： 
http://localhost:8081/index.android.bundle?platform=android 

4.遇到问题时候在cmd命令行运行 adb shell input keyevent 82
