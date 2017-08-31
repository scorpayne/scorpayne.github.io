---
title: Sublime Text 3 使用HTML-CSS-JS Prettify插件格式化代码
date: 2017-08-31 22:54:16
tags:
---
如果你想要在你的Sublime Text 3编辑器上格式化，HTML-CSS-JS代码，比如Html，json字符串等，可以安装**HTML-CSS-JS Prettify**插件来实现此功能！

## **准备工作**

### 一、安装 Package Control
Package Control是一个包安装管理工具，有了它就可以下载各种插件了
	
### 二、安装Node.js（HTML-CSS-JS Prettify插件基于Node.js）
`简介：`
Node.js是一个基于v8引擎，采用异步IO，事件驱动，构建web服务的后端轻量级架构，能让javascript运行在服务端的平台
    
`优点：`
V8引擎执行Javascript的速度非常快，Node.js对其进行了封装，轻量并高效，IO密集型分布式部署环境下的实时应用系统的完美解决方案

`Windows安装包（.msi）`
32位安装包下载地址：https://nodejs.org/dist/v6.2.0/node-v6.2.0-x86.msi
64位安装包下载地址 :https://nodejs.org/dist/v6.2.0/node-v6.2.0-x64.msi

## **安装执行**

### 一、打开package control的[官网](https://packagecontrol.io/installation)
**1.复制对应Sublime版本的安装代码，Sublime Text 3如下:**

```c
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

**2.使用快捷键 control+` ，打开sublime的命令输入框如图**
    
![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831115631.png)

**3.粘贴上述代码，回车**
    
![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831112947.png)

在Preferences菜单的二级菜单中出现Package Control说明安装成功了

**4.使用快捷键 Ctrl+Shift+P，输入install package，打开包管理器**
    
![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831113010.png)

**5.输入pretty，并在列表中选择HTML-CSS-JS Prettify后回车即可安装（已经安装过貌似找不到了- -）**

### 二、查看本地安装的NodeJS配置环境路径
**1.在Node.js安装成功的前提下，window下cmd进行命令行，输入where node**

![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831113611.png)

**2.在编辑器窗口任意地方反键，将路径粘贴到配置文件中保存**

![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831114434.png)

![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831114522.png)

**3.重启sublime，重载插件**

## 演示
`常用快捷键`
> * Ctrl+Shift+H:格式化代码
> * Ctrl+Shift+M:压缩代码

测试代码如下：

```js
{ "keys": [ "ctrl+alt+m" ], "command": "un_pretty_json" }
```

![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831115131.png)

使用快捷键Ctrl+Shift+H如下

![](https://raw.githubusercontent.com/scorpayne/MarkdownPhotos/master/blog/20170831115210.png)

------
作者 [scorpayne][1]
[1]: https://scorpayne.github.io/



