# Aath

Aath 参考了[知乎](https://www.zhihu.com/)和[掘金](https://juejin.im/timeline)的部分设计

## [Demo](http://lewis.suclub.cn/)

![Aath](http://olnzpdi2u.bkt.clouddn.com/flat-devices.png)

## 安装

###  主题

```bash
$ git clone -b master https://github.com/lewis-geek/hexo-theme-Aath.git themes/aath
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

# Comment
## disqus
disqus_shortname: your_disqus_shortname

#lewis-theme
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

## 特性

### fancybox

Aath 使用 [fancyBox](http://fancyapps.com/fancybox/) 浏览文章中的图片。

### catalog

自动为文章生成多级目录。

### markdown

使用 GitHub 的 markdown 样式。
