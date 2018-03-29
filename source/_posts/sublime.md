---
title: Sublime Text常用插件介绍及安装
tags: [Sublime Text,教程]
categories: Sublime Text

---

作为代码编辑器Sublime Text界面界面整洁美观、文本功能强大，且运行速度极快，非常适合编写代码，写文章做笔记。而且很多有功能强大的插件可以使用。
## 安装插件管理器 Package Control
（1)  在Sublime中打开View –> Show Console(或者用快捷键ctrl+~)，将以下代码复制到输入框中后按回车键
```
import urllib.request,os;pf=’Package Control.sublime-package’;
ipp=sublime.installed_packages_path();
urllib.request.install_opener(urllib.request.build_opener(urllib.request.ProxyHandler()));
open(os.path.join(ipp,pf),’wb’).write(urllib.request.urlopen(‘http://sublime.wbond.net/‘+pf.replace(’ ‘,’%20’)).read())
```
（2)  验证是否安装成功

打开Preferences –> Package Control,如果能看到此菜单，则表示安装成功

![1](/images/2.1.png)
## 如何安装插件
打开Preferences –> Package Control选择Install Package(快捷键shift+ctrl+p选择第一个选项也行)，然后在出现的输入框内输入你想安装的插件，找到后点击即可安装。下方状态栏会显示安装状态，安装完成会显示说明文档。下面是一些常用的插件。
![2](/images/2.2.png)
## 1.Ement
HTML/CSS代码快速编写插件。可以在其官网<a href="http://docs.emmet.io/">(http://docs.emmet.io/</a>)上看到具体的演示视频。可以用这个完成前端重复性的代码。
### 使用示例
`div#test>li*6`
然后ctrl+e生成

![3](/images/2.3.png)
## 2.JSFormat
Javascript的代码格式化插件，可以将一整行的JS原始代码进行整理，整理为带有换行和缩进的更容易看懂的代码。
使用：ctrl+Alt+F
## 3.Bracket Highlighter
代码匹配插件，可以匹配对应的（）{} [] ""，便于查看起始和结束。点击即会出现提示。
## 4.jQuery
jQuery函数代码提示。
这一类代码提示的还有AngularJS  NodeJs 等都可以使打代码变得更快捷。
## 5.ColorPicker
在需要输入颜色时，可以便捷选取颜色。
使用:ctrl+shift+c

效果如下

![4](/images/2.4.png)
## 6.Color Highlighter
展示代码真正的颜色。界面会看着更舒服更清楚。
## 7.SublimeLinter
检错插件，可以高亮提示认为有错误的代码行。
## 8.Alignment
代码对齐。可以整理写的不整齐的代码。
使用：选中要整理的部分，ctrl+alt+A，就可以对齐了。
注:快捷键与QQ热键冲突的，可以Preferences->Key Blindings，然后在右边输入框键入

```[
     {"keys": ["ctrl+alt+q"], "command": "reindent"},
]
```

keys设置为自己喜欢的快捷键，在这里示范的是ctrl+alt+q。也可以修改QQ的快捷键。

## 9.SublimeCodeIntel
代码自动提示补全。
## 如何查看自己已安装的插件
快捷键 ctrl+shift+p，在框中输入“list”，选择“Package Control:List Packages”。
会列出所有已安装的插件。
## 如何移除插件
快捷键 ctrl+shift+p，在框中输入“remove”，选择“Package Control: Remove Packages”。
然后在出现的插件列表中点选你要移除的插件。
