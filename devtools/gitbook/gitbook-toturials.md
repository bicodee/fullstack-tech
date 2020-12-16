# GitBook使用教程

## 命令行工具安装

### 安装node.js
gitbook cli是基于Node.js的命令行工具，需要先下载安装node.js

### 安装gitbook cli
最好的安装GitBook的方法是通过NPM。在终端提示符下，只需运行以下命令即可安装GitBook：
```
$ npm install gitbook-cli -g
```
gitbook-cli是在同一系统上安装和使用多个版本的GitBook的实用程序。它将自动安装所需版本的GitBook来构建一本书。

## 创建一本书
+ GitBook可以设置样板书：
```
$ gitbook init
```
如果您希望将图书创建到新目录中，可以通过运行 gitbook init ./directory

+ 使用以下方法预览和提供图书：
```
$ gitbook serve
```

+ 或使用以下方法构建静态网站：
```
$ gitbook build
```

## 目录结构
GitBook使用简单的目录结构。概要中列出的所有Markdown / Asciidoc文件都将转换为HTML。多语言书籍的结构略有不同。

基本的GitBook通常看起来像这样：
```
.
├── book.json
├── README.md
├── SUMMARY.md
├── chapter-1/
|   ├── README.md
|   └── something.md
└── chapter-2/
    ├── README.md
    └── something.md
```
#### book.json
用于存储配置信息（可选），简单可以理解为配置文件，后续会涉及。
#### README.md
用于描述前言/说明信息（必须），简单可以理解为主页，按照Markdown格式编写即可。
#### SUMMARY.md
用于描述章节列表（可选，建议必须），简单可以理解为导航栏，接下来会介绍。

## 常用命令
> npm install gitbook-cli -g ：安装gitbook-cli；
>
> gitbook ls ：列出本地安装版本；
>
> gitbook current ：列出当前使用版本；
>
> gitbook ls-remote ：列出远程可使用版本；
>
> gitbook fetch 2.6.9 ：安装2.6.9版本；
>
> gitbook uninstall 2.6.9 ：卸载指定版本；
>
> gitbook update 2.6.9 ：更新到指定版本，没有指定版本则到最新；
>
> gitbook install ：安装当前项目所需插件；
>
> gitbook build ：构建成Html文件，默认在_book目录下；
>
> gitbook serve：启动服务；
>
> gitbook pdf ：输出pdf电子书；
>
> gitbook epub：输出epub电子书；
>
> gitbook mobi ：输出mobi电子书；
>

## 常用工具

1. GitHub
2. Gitbook Editor
3. [Typora](https://typora.io/#)

## 常见问题

> ##### 问题1：GitBook生成PDF问题
> 问题描述：windows 系统 GitBook生成PDF、epub报错Error during ebook generation: 'ebook-convert' 乱码
>
> 解决方法：下载[calibre](https://calibre-ebook.com/)并安装，重新执行gitbook pdf命令。
>


## 附录
+ [GitBook 官网](https://www.gitbook.com)
+ [GitBook 文档](https://github.com/GitbookIO/gitbook)
+ [Gitbook editor与gitbook，github同步](https://blog.csdn.net/qq_35830949/article/details/79355530)
+ [windows安装gitbook并使用gitbook editor可视化工具](https://www.cnblogs.com/kingsonfu/p/10255123.html)
+ [Typora完全使用详解](https://sspai.com/post/54912/)