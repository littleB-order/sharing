
# GitBook {#main}

##### *TAG :* `Gitbook`

[<目录>](#main)
* [A. 安装](#installation)
    - [安装Node.js](#installation_1)
    - [安装NPM](#installation_2)
    - [安装Gitbook](#installation_3)
* [B. 使用](#serving)
    - [创建页面](#serving_1)
    - [预览页面](#serving_2)
    - [生成页面](#serving_3)
    - [更新页面](#serving_4)
* [C. 新建](#creation)
    - [新建文档](#creation_1)
    - [修改索引](#creation_2)

## A. 安装 {#installation}

### 安装Node.js {#installation_1}
```bash
# 安装Node.js
$ brew install node
# 检查当前版本
$ node -v
# 更新至最新版
$ brew upgrade node
```

### 安装NPM {#installation_2}
```bash
# 更新NPM
$ npm install npm@latest -g
# 检查NPM版本
$ npm -v
```

### 安装gitbook {#installation_3}
```bash
$ npm install gitbook-cli -g
```

###### [Back](#main)
---

## B. 使用 {#serving}

### 创建新的gitbook {#serving_1}
```bash
$ gitbook init
```

### 实时预览 {#serving_2}
```bash
# Serving book on http://localhost:4000
$ gitbook serve
```
[预览链接](http://localhost:4000)

### 生成页面 {#serving_3}
```bash
$ gitbook build
```

### 更新及上传  {#serving_4}
复制`_book`目录下所有文件至`sharing`根目录下，选择替换全部。


###### [Back](#main)
---

## C. 新建 {#creation}

### 新建文档 {#creation_1}
在`/sharing/docs/`目录的相关文件夹中创建`.md`的Markdown文件。

### 修改索引 {#creation_2}
更改`/sharing/docs/SUMMARY.md`以修改索引目录。每条链接对应一条索引。
```markdown
 * [项目](README.md) <= README.md为项目介绍，对应相应文件夹下的文件。
    * [子条目](文件名.md) <= 文件名对应项目文件夹下的文件。
```

###### [Back](#main)
---
