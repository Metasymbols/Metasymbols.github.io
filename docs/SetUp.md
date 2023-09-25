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

#### 系统偏好设置

通过使用媒体查询，每个调色板都可以链接到用户对浅色和深色外观的系统偏好。只需在以下定义旁边添加一个`media`属性：`scheme``mkdocs.yml`

```
theme:
  palette:

    # Palette toggle for light mode
    - media: "(prefers-color-scheme: light)"
      scheme: default
      toggle:
        icon: material/brightness-7
        name: Switch to dark mode

    # Palette toggle for dark mode
    - media: "(prefers-color-scheme: dark)"
      scheme: slate
      toggle:
        icon: material/brightness-4
        name: Switch to light mode

```
当用户第一次访问您的网站时，媒体查询将按照其定义的顺序进行评估。第一个匹配的媒体查询选择默认调色板。

#### 自动亮/暗模式


较新的操作系统允许在白天和夜间自动在浅色和深色外观之间切换。[Insiders](https://squidfunk.github.io/mkdocs-material/insiders/)增加了对自动亮/暗模式的支持，将调色板选择委托给用户的操作系统。将以下行添加到`mkdocs.yml`：

```
theme:
  palette:

    # Palette toggle for automatic mode
    - media: "(prefers-color-scheme)"
      toggle:
        icon: material/brightness-auto
        name: Switch to light mode

    # Palette toggle for light mode
    - media: "(prefers-color-scheme: light)"
      scheme: default 
      toggle:
        icon: material/brightness-7
        name: Switch to dark mode

    # Palette toggle for dark mode
    - media: "(prefers-color-scheme: dark)"
      scheme: slate
      toggle:
        icon: material/brightness-4
        name: Switch to system preference

```

#### 定制颜色

`[data-md-color-scheme="..."]` [除了覆盖特定颜色之外，您还可以通过将定义包装在属性选择器](https://www.w3.org/TR/selectors-4/#attribute-selectors)中来创建自己的命名配色方案，然后您可以按照[配色方案](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-scheme)`mkdocs.yml`部分中所述进行设置：[](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#color-scheme)

 [`docs/stylesheets/extra.css`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#custom-color-schemes-docsstylesheetsextracss) [`mkdocs.yml`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/#custom-color-schemes-mkdocsyml)

```
[data-md-color-scheme="youtube"] {
  --md-primary-fg-color:        #EE0F0F;
  --md-primary-fg-color--light: #ECB7B7;
  --md-primary-fg-color--dark:  #90030C;
}

```


```
theme:
	palette:
	    scheme: youtube
extra_css:
	- stylesheets/extra.css

```

此外，`slate`配色方案通过颜色函数定义其所有颜色`hsla`，并从 CSS 变量推导出其颜色`--md-hue`。您可以`slate`通过以下方式调整主题：
```
[data-md-color-scheme="slate"] {
  --md-hue: 210; 
}

```


### 更改字体

#### 常规字体

常规字体用于所有正文、标题以及基本上所有不需要等宽的内容。可以通过以下方式将其设置为任何有效的[Google 字体](https://fonts.google.com/)`mkdocs.yml`：

```
theme:
  font:
    text: Roboto

```
字体将以 300、400、400i和**700**_加载_


#### 等宽字体

_等宽字体_用于代码块，可以单独配置。就像常规字体一样，它可以通过以下方式设置为任何有效的[Google 字体](https://fonts.google.com/)`mkdocs.yml`：

```
theme:
  font:
    code: Roboto Mono

```

字体将在 400 中加载。


#### 自动加载

[如果您想阻止从Google Fonts](https://fonts.google.com/)加载字体（例如，为了遵守[数据隐私](https://developers.google.com/fonts/faq#what_does_using_the_google_fonts_api_mean_for_the_privacy_of_my_users)法规）并回退到系统字体，请将以下行添加到`mkdocs.yml`：

```
theme:
  font: false

```

### 定制化

#### 附加字体

如果您想从其他目的地加载（附加）字体或覆盖系统字体，您可以使用附加[样式表](https://squidfunk.github.io/mkdocs-material/customization/#additional-css)来添加相应的`@font-face`定义：

 [`docs/stylesheets/extra.css`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-fonts/#additional-fonts-docsstylesheetsextracss) [`mkdocs.yml`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-fonts/#additional-fonts-mkdocsyml)
```
@font-face {
  font-family: "<font>";
  src: "...";
}

```


```
extra_css:
  - stylesheets/extra.css

```

然后，该字体可以应用于特定元素，例如仅标题，或全局用作站点范围的常规或等宽字体：

常规

```
:root {
  --md-text-font: "<font>"; 
}

```

等宽
```
:root {
  --md-code-font: "<font>";
}

```
### 更改语言


#### 网站语言
您可以使用以下方式设置站点语言`mkdocs.yml`：
```
theme:
  language: zh

```

#### 站点语言选择器
如果您的文档有多种语言版本，则可以将指向这些语言的语言选择器添加到标题中。可以通过 定义替代语言`mkdocs.yml`。

```
extra:
  alternate:
    - name: English
      link: /en/ 
      lang: en
    - name: Deutsch
      link: /de/
      lang: de

```
以下属性可用于每种备用语言：

[`name`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#+alternate.name)

该属性的值在语言选择器内部用作语言名称，并且必须设置为非空字符串。

[`link`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#+alternate.link)

该属性必须设置为绝对链接，该链接也可能指向不一定由 MkDocs 生成的另一个域或子域。

[`lang`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#+alternate.lang)

此属性必须包含[ISO 639-1 语言代码](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)，并用于`hreflang`链接的属性，从而提高通过搜索引擎的可发现性。

#### 方向性

虽然可以读取多种语言`ltr`（从左到右），但 Material for MkDocs 还支持`rtl`从所选语言推导出来的（从右到左）方向性，但也可以通过以下方式进行设置：

```
theme:
  direction: ltr
```

#### 定制翻译
[如果您想自定义某种语言的某些翻译，只需按照主题扩展](https://squidfunk.github.io/mkdocs-material/customization/#extending-the-theme)指南并在文件夹中创建一个新的部分即可`overrides`。然后，导入该语言的[翻译](https://github.com/squidfunk/mkdocs-material/blob/master/src/templates/partials/languages/)作为后备，并仅调整您想要覆盖的翻译：

 [`overrides/partials/languages/custom.html`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#custom-translations-overridespartialslanguagescustomhtml) [`mkdocs.yml`](https://squidfunk.github.io/mkdocs-material/setup/changing-the-language/#custom-translations-mkdocsyml)
```
<!-- Import translations for language and fallback -->
{% import "partials/languages/de.html" as language %}
{% import "partials/languages/en.html" as fallback %} 

<!-- Define custom translations -->
{% macro override(key) %}{{ {
  "source.file.date.created": "Erstellt am", 
  "source.file.date.updated": "Aktualisiert am"
}[key] }}{% endmacro %}

<!-- Re-export translations -->
{% macro t(key) %}{{
  override(key) or language.t(key) or fallback.t(key)
}}{% endmacro %}

```

```
theme:
  language: custom

```

### 更改徽标和图标

安装 Material for MkDocs 时，您可以立即访问_8,000 多个图标_，这些图标可用于自定义主题的特定部分和/或在 Markdown 中编写文档时使用。不够？您还可以轻松添加[其他图标。](https://squidfunk.github.io/mkdocs-material/setup/changing-the-logo-and-icons/#additional-icons)

#### 标识

徽标可以更改为位于文件夹中的用户提供的图像（任何类型，包括`*.png`和） ，或与主题捆绑的任何图标。将以下行添加到：
```
theme:
  logo: assets/logo.png

```

```
theme:
  icon:
    logo: material/library 

```

通常，页眉和侧边栏中的徽标链接到文档的主页，与`site_url`. 可以通过以下配置更改此行为：

```
extra:
  homepage: https://example.com

```

#### 网站图标
可以将图标更改为指向用户提供的图像的路径，该图像必须位于该`docs`文件夹中。将以下行添加到`mkdocs.yml`：

```
theme:
  favicon: images/favicon.png

```

您在网站上看到的大多数图标（例如导航图标）也可以更改。例如，要更改页脚中的导航箭头，请将以下行添加到`mkdocs.yml`：

```
theme:
  icon:
    previous: fontawesome/solid/angle-left
    next: fontawesome/solid/angle-right

```

以下是主题使用的可自定义图标的完整列表：

|图标名称|目的|
|---|---|
|`logo`|查看[标志](https://squidfunk.github.io/mkdocs-material/setup/changing-the-logo-and-icons/#logo)|
|`menu`|打开抽屉|
|`alternate`|改变语言|
|`search`|搜索图标|
|`share`|分享搜索|
|`close`|重置搜索，关闭公告|
|`top`|返回顶部按钮|
|`edit`|编辑当前页面|
|`view`|查看页面源代码|
|`repo`|存储库图标|
|`admonition`|请参阅[警告图标](https://squidfunk.github.io/mkdocs-material/reference/admonitions/#admonition-icons)|
|`tag`|请参阅[标签图标和标识符](https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/#tag-icons-and-identifiers)|
|`previous`|页脚中的上一页，隐藏移动设备上的搜索|
|`next`|页脚中的下一页|


#### 附加图标
为了使用自定义图标，[请扩展主题](https://squidfunk.github.io/mkdocs-material/customization/#extending-the-theme)`.icons`并创建一个以要[`custom_dir`](https://www.mkdocs.org/user-guide/configuration/#custom_dir)用于覆盖的名称命名的新文件夹。接下来，将`*.svg`图标添加到该`.icons`文件夹​​的子文件夹中。假设您下载并解压了[Bootstrap](https://icons.getbootstrap.com/)图标集，并希望将其添加到您的项目文档中。您的项目的结构应该如下所示：

![[Pasted image 20230925154538.png]]

然后，将以下行添加到`mkdocs.yml`：

```
markdown_extensions:
  - pymdownx.emoji:
      emoji_index: !!python/name:material.extensions.emoji.twemoji
      emoji_generator: !!python/name:material.extensions.emoji.to_svg
      options:
        custom_icons:
          - overrides/.icons


```

您现在可以使用所有Markdown 文件中任意位置的 Bootstrap 图标，以及可在`mkdocs.yml`. 但请注意，语法略有不同：

- **在配置中使用图标**`*.svg`：获取从文件夹开始的图标文件的路径`.icons`并删除文件扩展名，例如对于`.icons/bootstrap/envelope-paper.svg`，使用：
```
theme:
  icon:
    logo: bootstrap/envelope-paper
```

**在 Markdown 文件中使用图标**`.icons`：除了从上述文件夹中获取路径之外，将全部替换`/`为`-`并将图标短代码括在两个冒号中：
```
:bootstrap-envelope-paper:
```

### 确保数据隐私


#### Cookie 同意

MkDocs 的材料附带了一个本机且可扩展的 cookie 同意书，该同意书在向第三方发送请求之前请求用户同意。将以下内容添加到`mkdocs.yml`：

```
extra:
  consent:
    title: Cookie consent
    description: >- 
      We use cookies to recognize your repeated visits and preferences, as well
      as to measure the effectiveness of our documentation and whether users
      find what they're searching for. With your consent, you're helping us to
      make our documentation better.

```