# 配置


MkDocs 的材料提供了广泛的选项来自定义您的文档。在本节中，我们将解释如何为您的网站创建有意义的结构，更改外观，添加博客和评论系统，以及构建高度优化的网站。


## 网站结构

通过根据您的喜好配置页眉和页脚、在多种导航模式中进行选择、设置站点搜索等，设置和自定义文档的结构。


-  **[语言](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/)**– 从 60 多种支持的语言中选择或添加新语言
-  **[导航](https://squidfunk.github.io/mkdocs-material/setup/setting-up-navigation/)**——创建清晰、简洁、全面的导航结构
-  **[标题](https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-header/)**- 自定义标题的行为，添加公告栏
-  **[页脚](https://squidfunk.github.io/mkdocs-material/setup/setting-up-the-footer/)**- 在页脚中添加指向您的社交媒体资料或网站的链接
-  **[搜索](https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-search/)**– 设置和配置搜索，完全在用户浏览器中运行
-  **[标签](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/)**- 使用标签对页面进行分类并对相关页面进行分组

## 外观

通过几行配置来匹配您品牌的颜色、字体、图标、徽标等 - Material for MkDocs 可以轻松扩展基本配置或更改外观。

-  **[颜色](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/)**使用现有调色板更改颜色或使用 CSS 自定义
-  **[字体](https://squidfunk.github.io/mkdocs-material/setup/changing-the-fonts/)**– 从 1,000 种 Google 字体中进行选择或加载自托管字体
-  **[徽标和图标](https://squidfunk.github.io/mkdocs-material/setup/changing-the-logo-and-icons/)**– 更改徽标、使用 8,000 多个图标中的任何一个或添加新图标
-  **[社交卡](https://squidfunk.github.io/mkdocs-material/setup/setting-up-social-cards/)**- 共享链接时自动创建社交媒体预览

## 内容

创建博客、集成评论系统、连接 git 存储库，并设置与项目的版本控制方法相匹配的版本化文档。

-  **[博客](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/)**– 设置独立博客或将其与文档一起托管
-  **[评论系统](https://squidfunk.github.io/mkdocs-material/setup/adding-a-comment-system/)**- 在任何页面或页脚添加第三方评论系统
-  **[版本控制](https://squidfunk.github.io/mkdocs-material/setup/setting-up-versioning/)**– 通过与外部实用程序集成来部署多个版本
-  **[存储库](https://squidfunk.github.io/mkdocs-material/setup/adding-a-git-repository/)**– 将您的文档连接到 git 存储库

## 优化

添加站点分析并通过添加自动图像压缩、遵守 GDPR 数据隐私法规并使其具有离线功能来构建优化的站点。

-  **[站点分析](https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-analytics/)**– 了解您的用户如何体验您的文档
-  **[优化网站](https://squidfunk.github.io/mkdocs-material/setup/building-an-optimized-site/)**– 创建在搜索引擎上排名靠前的优化网站
-  **[数据隐私](https://squidfunk.github.io/mkdocs-material/setup/ensuring-data-privacy/)**– 确保遵守数据隐私法规
-  **[离线使用](https://squidfunk.github.io/mkdocs-material/setup/building-for-offline-usage/)**– 构建可在线和离线使用的文档



### 改变颜色

与任何适当的 Material Design 实现一样，Material for MkDocs 支持 Google 的原始[调色板](http://www.materialui.co/colors)，可以通过 轻松配置`mkdocs.yml`。[此外，还可以使用CSS 变量](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#custom-colors)通过几行 CSS 来自定义颜色，以适应您的品牌标识。

#### 调色板

配色方案
Material for MkDocs 支持两种配色方案：**浅色模式**（称为 ）`default`和**深色模式（**称为 ）`slate`。配色方案可以通过以下方式设置`mkdocs.yml`：

```
theme:
  palette:
    scheme: default

```

###### 原色

原色用于标题、侧边栏、文本链接和其他几个组件。要更改主颜色，请将以下值设置`mkdocs.yml`为有效的颜色名称：
```
theme:
  palette:
    primary: indigo

```

单击图块以更改主颜色：

`red` `pink` `purple` `deep purple` `indigo` `blue` `light blue` `cyan` `teal` `green` `light green` `lime` `yellow` `amber` `orange` `deep orange` `brown` `grey` `blue grey` `black` `white`

请参阅下面的指南，了解如何设置[自定义颜色](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#custom-colors)。


###### 强调色
强调色用于表示可以交互的元素，例如悬停的链接、按钮和滚动条。`mkdocs.yml`可以通过选择有效的颜色名称来更改它：
```
theme:
  palette:
    accent: indigo

```

单击图块可更改强调色：

`red` `pink` `purple` `deep purple` `indigo` `blue` `light blue` `cyan` `teal` `green` `light green` `lime` `yellow` `amber` `orange` `deep orange`

请参阅下面的指南，了解如何设置[自定义颜色](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#custom-colors)。

#### 调色板切换
提供浅色_和_深色调色板使您的文档在一天中的不同时间都易于阅读，因此用户可以进行相应的选择。将以下行添加到`mkdocs.yml`：
```
theme:
  palette: 

    # Palette toggle for light mode
    - scheme: default
      toggle:
        icon: material/brightness-7 
        name: Switch to dark mode

    # Palette toggle for dark mode
    - scheme: slate
      toggle:
        icon: material/brightness-4
        name: Switch to light mode

```

此配置将在搜索栏旁边呈现调色板切换。请注意，您还可以为每个调色板定义单独的[`primary`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#primary-color)设置[`accent`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#accent-color)。

必须为每个切换设置以下属性：
[`icon`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#+palette.toggle.icon)

[此属性必须指向引用与主题捆绑的任何图标的有效图标路径，否则构建将不会成功。一些流行的组合：

- +– `material/brightness-7`+`material/brightness-4`
- +– `material/toggle-switch`+`material/toggle-switch-off-outline`
- +– `material/weather-night`+`material/weather-sunny`
- +– `material/eye`+`material/eye-outline`
- +– `material/lightbulb`+`material/lightbulb-outline`

[`name`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#+palette.toggle.name)

此属性用作切换的`title`属性，应设置为可识别的名称以提高可访问性。它呈现为[工具提示](https://squidfunk.github.io/mkdocs-material/reference/tooltips/)。


