# Aath

[中文文档](https://github.com/lewis-geek/hexo-theme-Aath/blob/develop/README.md)

Aath refers to the partial design of [zhihu](https://www.zhihu.com/) and [juejin](https://juejin.im/timeline).

## [Demo](http://lewis.suclub.cn/)

### [test site](https://lewis-geek.github.io/hexo-theme-unit-test/)

### [code samples](https://github.com/lewis-geek/hexo-theme-unit-test)

![Aath](http://cdn.suclub.cn/Untitled-1880.png)

## Installation

### Theme

#### latest release

```bash
$ git clone -b master https://github.com/lewis-geek/hexo-theme-Aath.git themes/aath
```

#### beta version

```bash
$ git clone -b develop https://github.com/lewis-geek/hexo-theme-Aath.git themes/aath
```

### Dependence

```bash
$ npm install --save hexo-renderer-sass
```

## Configuration

There are two configuration files for hexo, one in the root directory of the hexo project and the other in the root directory of the theme folder. The file names are both `_config.yml`.

### Project Configuration

```yaml
Theme: aath

# highlight
## line_number
Highlight:
  Line_number: false

# Comment
## disqus
## livere
Disqus_shortname: your_disqus_shortname
Livere_uid: your_livere_uid

# favicon
Favicon: /favicon.ico

# Aside
## search
## avatar
## aside-description
## links
Search: true
Avatar: http://olnzpdi2u.bkt.clouddn.com/avatar.jpg
Aside-description: aside-description
Links:
  Baidu: https://www.baidu.com/
  Google: https://www.google.com/
  Zhihu: https://www.zhihu.com/
```

### topic configuration

```yaml
# main menu navigation
Menu:
  Home: /
  About: /about
  Archive: /archives
  Tags: /tags

# Miscelaneous
Favicon: /favicon.ico
```

### About page

If you need to generate the about page, you need to create an about directory in the source directory and create an index.md file in the about directory to add the `layout: about` attribute to the file. You can access the about page in the `<your_url>/about` path.

### Tags page

If you need to generate tags pages, you need to create a tags directory in the source directory, create an index.md file in the tags directory, and add the `layout: tags` attribute to the file. At this point you can access the tags page in the `<your_url>/tags` path.

## Features

### fancybox

Aath used [fancyBox](http://fancyapps.com/fancybox/) to browse through the pictures in the article.

### Article Directory

Automatic generation of multi-level directories for the article. The directory style uses the `position: sticky` attribute, which achieves a fixed directory-browser effect. This is a newer attribute and requires browser support.

### markdown

Use the GitHub's markdown style.

### Article list

#### Article Image

Add the `img` attribute at the top of the markdown file. The attribute value is the picture address.

#### Article description

Add the `description` attribute at the top of the markdown file to display the description of the article in the top article list. If there is no such attribute, the article content will be automatically intercepted as a description of the article.
