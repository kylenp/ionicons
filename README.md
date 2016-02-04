# Ionicons - 为设计而生


专为 [Ionic Framework](http://ionicframework.online/) 设计的图标字体库

    说明：所有品牌图标的版权仍归品牌厂商所有。

你可以在 [ionicons.online](http://ionicons.online) 浏览所有图标字体并了解如何使用，还可以使用关键词快速搜索你需要的图标或样式。

例如，搜索 “arrow” 关键词会显示返回按钮、箭头指示等图标，点击对应的图标可以快速复制图标样式，将它 复制/粘贴 到你的代码中即可！

虽然 Ionicons 是专为 [Ionic Framework](http://ionicframework.online/) 设计，但并不仅限于在 Ionic 项目中才能使用。相反，你可以在任何场合及项目中使用它们，你只需要在项目中引用图标字体库样式，就这么简单！

现在，我们已经将项目开源并使用 [MIT](http://opensource.org/licenses/MIT) 授权许可协议。


## 开始使用

 1. 下载并解压图标字体库；
 2. 将 `ionicons.css` 文件复制到项目样式资源目录；
 3. 将 `fonts` 文件夹下的字体文件复制到项目字体资源目录（当然，你也可以直接把 `fonts` 文件夹复制到项目并作为项目字体资源目录）；
 4. 确保 `ionicons.css` 中字体资源路径与项目中 `fonts` 目录路径保持一致；
 5. 在页面中引用 `ionicons.css` 文件，开始使用图标字体！

你还可以使用 [component](https://github.com/componentjs/component) 安装：

    $ component install vultur/ionicons
    
再或者使用  [bower](http://bower.io/) 安装：
   
    $ bower install ionicons


## 演示示例

你可以在 [ionicons.online](http://ionicons.online) 浏览或搜索需要的图标字体，你只需要在 HTML 元素的类名中添加 `icon` 字段和图标样式即可。例如，显示图标样式为 `ion-home` 的图标字体：

    <i class="icon ion-home"></i>


## 如何自定义图标字体？

This repo already comes with all the files built and ready to go, but can also build the fonts from the source. Requires Python, FontForge and Sass:

1) 安装 FontForge， 并将 SVG 转换为字体文件：

    $ brew install fontforge ttfautohint

2) 安装 [Sass](http://sass-lang.com/) 样式处理器：

    $ gem install sass

3) 在 `src/` 目录下添加或删除需要合并的字体文件；

4) 在 `builder/manifest.json` 文件中修改字体名称和图标样式名称；

5) 编译并生成新的图标字体库：

    python ./builder/generate.py


## 许可协议

使用 [MIT](http://opensource.org/licenses/MIT) 授权许可协议



