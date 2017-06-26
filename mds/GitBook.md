\[TOC\]

# GitBook

GitBook就是用git+markdown来编写书籍的解决方案!

GitBook 是开源的，地址：[https://github.com/GitbookIO/gitbook](https://github.com/GitbookIO/gitbook)

# 编辑操作

GitBook 主要有三种编辑途径，通过git功能可以相互交替使用。

## ①命令 + Markdown

```shell
//初始化目录文件
  gitbook init
//生成静态网页
  gitbook build
//开启服务在浏览其中预览
  gitbook serve

gitbook update //更新到gitbook的最新版本
gitbook uninstall 2.0.1 //卸载对应的gitbook版本

gitbook help //列出gitbook所有的命令
gitbook --help //输出gitbook-cli的帮助信息
gitbook ls //列出本地所有的gitbook版本
gitbook ls-remote //列出远程可用的gitbook版本
gitbook fetch 标签/版本号 //安装对应的gitbook版本
```

```shell
Last login: Wed Jun 21 09:07:26 on console
172-3-200-128:~ Alfred$ cd /Users/Alfred/Desktop/book  # 创建一个文件夹
172-3-200-128:book Alfred$ gitbook init  # gitbook init
warn: no summary file in this book 
info: create README.md 
info: create SUMMARY.md 
info: initialization is finished 
172-3-200-128:book Alfred$ gitbook init
info: create SUMMARY.md 
info: initialization is finished 
172-3-200-128:book Alfred$ gitbook build  # gitbook build
info: 7 plugins are installed 
info: 6 explicitly listed 
info: loading plugin "highlight"... OK 
info: loading plugin "search"... OK 
info: loading plugin "lunr"... OK 
info: loading plugin "sharing"... OK 
info: loading plugin "fontsettings"... OK 
info: loading plugin "theme-default"... OK 
info: found 4 pages 
info: found 0 asset files 
info: >> generation finished with success in 1.2s ! 

172-3-200-128:book Alfred$ gitbook serve  # gitbook serve
Live reload server started on port: 35729
Press CTRL+C to quit ...  #gitbook CTRL+C

info: 7 plugins are installed 
info: loading plugin "livereload"... OK 
info: loading plugin "highlight"... OK 
info: loading plugin "search"... OK 
info: loading plugin "lunr"... OK 
info: loading plugin "sharing"... OK 
info: loading plugin "fontsettings"... OK 
info: loading plugin "theme-default"... OK 
info: found 4 pages 
info: found 0 asset files 
info: >> generation finished with success in 0.7s ! 

Starting server ...
Serving book on http://localhost:4000
Serving book on http://localhost:4000
^C  # Control+C退出监控   
172-3-200-128:book Alfred$
```

运行`gitbook build`后，在你的图书项目的目录中多了一个名为`_book`的文件目录，这个目录中的文件即是生成的静态  
网站内容。

```shell
# 使用build参数生成到指定目录
$ gitbook build --output=/tmp/gitbook
```

通过服务器监控，然后通过第三方markdwon编辑器（例如，MacDown、马克飞象，typora等）进行文件修改；每次修改保存是，监控的服务器都会即使响应更新，及时可以预览变化。

### 本地如何关联GitBook Editor 或GitBook.io?

如果想切换到用GitBook Editor来编辑，首先要将你的书关联到一个git仓库（例如：[https://git.gitbook.com/cwlife/iweb.git](https://git.gitbook.com/cwlife/iweb.git) 或者github仓库[https://git.oschina.net/alfred03/book-axyz.git）；然后通过'GitBook\)\)\](https://git.oschina.net/alfred03/book-axyz.git）；然后通过'GitBook%29%29\)\) Editor'的'Import'导入GitBook Editor进行编辑修改并可以上传到仓库。

> 建议：先建仓库，然后克隆至本地！

## ②GitBook Editor

可以：

* 新建书籍

* 编辑书籍

  ![](https://ws4.sinaimg.cn/large/006tNc79gy1fgso574948j30k402maab.jpg)

* 上传书籍

* 可以修改仓库地址：菜单-'BOOK'-'Repository Settings'

![菜单-&apos;BOOK&apos;-&apos;Repository Settings&apos;](https://ws2.sinaimg.cn/large/006tNc79gy1fgsn8ah40fj30eh09475t.jpg)

也可以直接打开本地文件夹，用markdown编辑器编辑单个文件，保存修改时，会弹出如下提示，选择同步‘Sync’可以保存修改：

![选择同步‘Sync’可以保存修改](https://ws4.sinaimg.cn/large/006tNc79gy1fgsnbndj4pj30hq07tgma.jpg)

## ③GitBook.io

GitBook.io/GitBook.com

包含所有功能的操作。

其中，"Settings"这个栏目可以做很多设置，例如将书籍重命名：

![](/images/options.png)

### 找书:explore板块

网址：[https://www.gitbook.com/explore](https://www.gitbook.com/explore)

在这个版块，你可以搜索开放的书籍。

```java
https://www.gitbook.com/@xiaolai  #李笑来的
https://www.gitbook.com/@wizardforcel # 很多IT的书
https://www.gitbook.com/@yourtion
```

​

# 关联GitHub

在 GitHub 上创建一个仓库，来管理书籍源码。将 gitbook.com 上的电子书与 GitHub 的远程仓库关联起来；这样，相互的修改都可以同步保存。

登陆 gitbook.com 网站，可以看到我们之前创建的电子书，然后点击 "Book Settings" 按钮。

![img](https://dn-anything-about-doc.qbox.me/document-uid53532labid2137timestamp1474446591331.png/wm)

在 "Settings" 栏目中，点击 "GitHub"。

![img](https://dn-anything-about-doc.qbox.me/document-uid53532labid2137timestamp1474446609335.png/wm)

点击 "Select a Repository"，选择我们创建的存放电子书源码的仓库。

![img](https://dn-anything-about-doc.qbox.me/document-uid53532labid2137timestamp1474446637713.png/wm)

确定仓库之后，点击 "Sync" 按钮，同步。

![](https://ws3.sinaimg.cn/large/006tNc79gy1fgso0b3v84j30tb0m2aco.jpg)

![img](https://dn-anything-about-doc.qbox.me/document-uid53532labid2137timestamp1474446898021.png/wm)

成功！之后，每次在 GitHub 上更新电子书时，都会自动同步到 gitbook.com，并且自动编译成电子书。

# 插件安装与配置

Gitbook 本身功能丰富，可以使用插件来进行个性化定制。[Gitbook 插件](http://localhost:4000/start/plugin.html) 里已经有100多个插件，可以在 `book.json` 文件的 `plugins` 和`pluginsConfig` 字段添加插件及相关配置，添加后别忘了进行安装。

&gt;ps: 插件的效果是在生成电子书或网页时生效！

```json
// book.json
{
  "title": "Webpack 中文指南",
  "description": "Webpack 是当下最热门的前端资源模块化管理和打包工具，本书大部分内容翻译自 Webpack 官网。",
  "language": "zh",
  "plugins": [
    "disqus",
    "github",
    "editlink",
    "prism",
    "-highlight",
    "baidu",
    "splitter",
    "sitemap"
  ],
  "pluginsConfig": {  # 插件配置
    "disqus": {
      "shortName": "webpack-handbook"
    },
    "github": {
      "url": "https://github.com/zhaoda/webpack-handbook"
    },
    "editlink": {
      "base": "https://github.com/zhaoda/webpack-handbook/blob/master/content",
      "label": "编辑本页"
    },
    "baidu": {
        "token": "a9787f0ab45d5e237bab522431d0a7ec"
    },
    "sitemap": {
        "hostname": "http://zhaoda.net/"
    }
  }
}

# 安装插件
$ gitbook install ./
```

搜索插件: [GitBook Plugins](https://plugins.gitbook.com/browse)

* 代码高亮: [prism插件](https://plugins.gitbook.com/plugin/prism)
* 页面目录：
  * 页面内 - [navigator](https://plugins.gitbook.com/plugin/navigator)
  * 侧边 - [simple-page-toc](https://plugins.gitbook.com/plugin/simple-page-toc)
  * TOC 目录: [atoc](https://plugins.gitbook.com/plugin/atoc)

# 输出：

Gitbook网站上可以直接导出PDF，MOBI，EBUP等电子书格式

## 网页

## 输出PDF文件

先要使用NPM安装上gitbook pdf：

> $ sudo npm install gitbook-pdf -g

## gitbook epub

## gitbook mobi



