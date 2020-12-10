# GitBook使用教程

## GitBook命令行工具安装

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

## 附录
+ [GitBook 官网](https://www.gitbook.com)
+ [GitBook 文档](https://github.com/GitbookIO/gitbook)