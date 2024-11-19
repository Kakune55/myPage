# 文档编写规范
此文档用于描述文档编写规范，包括文档的格式、结构、内容等。
##命名规范
文件名使用横线命名法，如：`doc-spec.md`
采用英语描述文件内容

## Docsify
此文档使用 [Docsify](https://docsify.js.org/#/) 作为文档生成工具。
Docsify 是一个轻量级的静态网站生成器，使用 Markdown 格式编写文档，并生成静态页面。
帮助文档生成工具可以参考 [Docsify 官方文档](https://docsify.js.org/#/zh-cn/)

## Markdown
段落以空行分隔，段落之间以空行分隔。
段落内使用空格缩进，缩进为4个空格或一个制表符。
列表内使用空格缩进，缩进为2个空格或一个制表符。
语法需要符合Markdown规范
 1. [Markdown官方文档 (推荐)](https://markdown.com.cn/basic-syntax)
 2. [Markdown语法规范](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)
 3. [Markdown语法参考](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

## 组织结构
采用文件夹结构来表示文档的层级关系。
特殊文件：
- README.md：文档的入口，用于快速了解文档的功能，作为导航页使用  
访问URL：为目录结构+```/```  
  - 如本页面的上级目录为```/interior/tech/edit/```
  - 入口文件为```/interior/tech/edit/README.md```
  - 访问URL为```/interior/tech/edit/```
- _sidebar.md：侧边栏导航文件，用于快速定位文档,没有的话则继承上级目录
- _navbar.md：顶部导航文件，用于快速定位文档,没有的话则继承上级目录
- _sidebar.md 和 _navbar.md 均使用Markdown语法的无序列表

## 附件管理
附件目录，用于管理附件，如图片、视频等，默认为```/media```
- 图片存放在```/media/img```
- 视频存放在```/media/video```
存放路径需要与引用文件所处目录路径一致，如：
```/interior/tech/edit/README.md```引用图片为```logo.png```
则需要存放在```/interior/edit/media/img/logo.png```
~~~md
[logo](/interior/edit/media/img/logo.png)
~~~

## 附件限制
- 图片
  - 大小尽可能小于512K,格式为Webp 75质量压缩：```webp -q 75```(压缩方法参见:[文档编写工具-压制](/interior/tech/edit/tool?id=压制))
  - 分辨率在保证清晰的前提下，尽量不宜过大，16:9图片建议在1920*1080左右。
- 视频
  - 暂无 
