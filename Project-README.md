# 手册开发管理操作说明

协同编辑该手册项目的操作流程如下：

## 安装Node.js

下载安装Node.js

强烈推荐安装12.16.3版本Node.js，否则可能由于版本兼容问题导致无法启动GitBook服务

[12.16.3版本下载链接](https://nodejs.org/dist/v12.16.3/node-v12.16.3-x64.msi)

## 安装Gitbook

我们在cmd控制台可直接安装gitbook和检查版本，输入如下：

```bash
npm install gitbook-cli -g

gitbook -V
```

> CLI version: 2.3.2
> GitBook version: 3.2.3

参考gitbook的GitHub地址：[Setup and Installation of GitBook](https://github.com/GitbookIO/gitbook/blob/master/docs/setup.md)

## 安装VSCode及Markdown插件

为快速编辑和预览Markdown语法的用户手册内容，推荐使用VSCode作为集成开发环境

***推荐安装插件：***

- markdownlint
- Markdown Preview Enhanced

## 从Gitlab拉取产品手册项目代码

初始项目无Git地址（可跳过），后面根据项目需要自行申请手册Git管理

```bash
git clone 
```

## 安装依赖包

在cmd控制台进入该项目文件夹，安装依赖包：

```bash
yarn install
```

安装完成后会在当前项目目录下生产node_modules文件夹

## 替换样式代码

为实现手册自定义样式优化调整，需将src目录下的文件夹拷贝到本地目录node_modules下并覆盖原有文件

## 启动服务和Build发布

本地启动服务预览，执行以下命令：

```bash
gitbook serve
```

等待数秒，可看到如下信息，在浏览器可直接输入URL查看：

> Starting server ...
> Serving book on `http://localhost:4000`

Build发布为HTML文件，执行以下命令：

```bash
gitbook build
```

## Markdown语法手册

Markdown语法参考：[语法参考](https://www.jianshu.com/p/ebe52d2d468f)
