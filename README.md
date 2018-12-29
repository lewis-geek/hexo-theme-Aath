# Aath

[English Documentation](https://github.com/lewis-geek/hexo-theme-Aath/blob/develop/README.en.md)

Aath 参考了[知乎](https://www.zhihu.com/)和[掘金](https://juejin.im/timeline)的部分设计

## [Demo](http://lewis.suclub.cn/)

### [测试页面](https://lewis-geek.github.io/hexo-theme-unit-test/)

### [代码例子](https://github.com/lewis-geek/hexo-theme-unit-test)

![Aath](http://cdn.suclub.cn/Untitled-1880.png)

## 安装

### 主题

#### 最新 release 版

```bash
$ git clone -b master https://github.com/lewis-geek/hexo-theme-Aath.git themes/aath
```

#### 开发版

```bash
$ git clone -b develop https://github.com/lewis-geek/hexo-theme-Aath.git themes/aath
```

### 依赖

```bash
$ npm install --save hexo-renderer-sass
```

## 配置

hexo 有两个配置文件，一个在 hexo 项目的根目录，另一个在主题文件夹的根目录，文件名都是均为 `_config.yml` 。

### 项目配置

```yaml
theme: aath

# highlight
## line_number
highlight:
  line_number: false

# Comment
## disqus
## livere
disqus_shortname: your_disqus_shortname
livere_uid: your_livere_uid

# favicon
favicon: /favicon.ico

# Aside
## search
## avatar
## aside-description
## links
search: true
avatar: http://olnzpdi2u.bkt.clouddn.com/avatar.jpg
aside-description: aside-description
links:
  百度: https://www.baidu.com/
  谷歌: https://www.google.com/
  知乎: https://www.zhihu.com/
```

### 主题配置

```yaml
# main menu navigation
menu:
  首页: /
  关于: /about
  归档: /archives
  标签: /tags

# Miscelaneous
favicon: /favicon.ico
```

### About 页面

如果需要生成 about 页面，需要在 source 目录下创建一个 about 目录，并在 about 目录下创建一个 index.md 文件，为该文件添加 `layout: about` 属性。此时就可在 `<your_url>/about` 路径访问到 about 页面了。

### Tags 页面

如果需要生成 tags 页面，需要在 source 目录下创建一个 tags 目录，并在 tags 目录下创建一个 index.md 文件，为该文件添加 `layout: tags` 属性。此时就可在 `<your_url>/tags` 路径访问到 tags 页面了。

## 特性

### fancybox

Aath 使用 [fancyBox](http://fancyapps.com/fancybox/) 浏览文章中的图片。

### 文章目录

自动为文章生成多级目录，目录样式使用了 `position: sticky` 属性，实现了目录相对浏览器固定的效果，这是一个较新的属性，需要浏览器支持。

### markdown

使用 GitHub 的 markdown 样式。

### 文章列表

#### 文章图片

在 markdown 文件顶部添加 `img` 属性，属性值为图片地址。

#### 文章描述

在 markdown 文件顶部添加 `description` 属性，可以在首页文章列表显示文章的描述，如果没有这个属性，会自动截取文章内容作为文章的描述。
