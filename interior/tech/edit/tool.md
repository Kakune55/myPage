# 文档编写工具
此文档是关于文档编写的工具。
## Markdown编辑器
### 使用VSCode+Markdown All in One(推荐)
1. 下载并安装VSCode
- [VSCode官网](https://code.visualstudio.com)
- [镜像下载](https://www.baihezi.com/vscode/download)
下载完后运行安装包，选择安装。
2. 本地化配置
左侧菜单中点击 extensions，搜索```简体中文```，找到该插件，点击安装。并配置完成后，重启VSCode。
3. 安装Markdown All in One插件
[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
在```扩展```搜索框中输入`Markdown All in One`，选择`Markdown All in One`，点击`Install`即可。
![vscode-markdown](/media/img/vscode-markdown.webp)
4. 安装Live Server插件
[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
在```扩展```搜索框中输入`Live Server`，选择`Live Server`，点击`Install`即可。
### 使用其他Markdown编辑器
1. [MarkText](https://github.com/marktext/marktext)
2. [Typora](https://typora.io/)
3. [StackEdit](https://stackedit.io/)

## Git配置
### Git安装配置
[Git下载地址](https://git-scm.com/downloads)
[镜像下载](https://mirrors.tuna.tsinghua.edu.cn/github-release/git-for-windows/git/LatestRelease/)
版本区别：
- Git：完整版Git，包含Git Bash、Git GUI等命令行工具，通过安装包安装。
- MinGit：轻量版Git，只包含Git基本功能，通过手动。
- PortableGit：便携版Git 可供移动存储设备安装。  

本文档使用MinGit作为演示，配合VSCode使用。
1. 下载MinGit压缩包，解压到要安装Git的位置。如```MinGit-2.46.2-64-bit.zip```
2. 将Git目录中的cmd目录添加到环境变量中。如图：
![GitToPath](/media/img/config-path.webp)
3. 打开cmd，输入```git --version``` 如果出现版本信息，则安装成功。
~~~bash
> git --version
git version 2.45.1.windows.1
~~~

## 开始编辑
选择一个要存放编辑的文件夹的目录 如```D:\Documents```
1. 打开CMD，输入```git clone <仓库地址>```(仓库地址见文章底部)
2. 打开VSCode，左上角 文件 > 打开文件夹 > 刚刚克隆好的文件夹
3. 即可开始编辑，编辑规范参见[文档编写规范](/interior/tech/edit/spec)

## 压制
上传的媒体素材需要压制：
### 图片WebP压制
下面提供几种压制方法：
1. 在线转换：[在线工具](https://onlineconvertfree.com/zh/convert-format/png-to-webp/)
2. 使用ffmpeg：```ffmpeg -i <input> -q 75 <output>```
3. 使用其他工具

## Git仓库
待补充