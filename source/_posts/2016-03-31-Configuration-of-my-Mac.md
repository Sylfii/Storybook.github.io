---
title: Configuration of my Mac
date: 2016-03-31 18:54:48
tags: 
- Mac
- Application
---
For my friends, and the unknown you.

It's hart to say Mac OS X is friendly, since I have to  Z-Turn with it now and then. However, the grass is always greener on the other side of the hill. I believe if I used Win instead of Mac, there wouldn't be any difference.

This post is about my Mac's 'infrastructure', in case that I have to configure another one...

*IF YOU CAN'T UNDERSTAND CHINESE, PLESE STOP HERE OR EMAIL <a href="mailto:sylfii@outlook.com">ME</a>.*
<!-- more -->

# 闲言篇

呼~，终于可以回来写中文了！其实我也很想全部用英语的，可是那样比较耗时.....另外，相信我为数不多的读者也一定都是汉语使，再继续用英语也只是徒增彼此的烦恼啦~

记忆最深的高三时期的两任同桌、远在海外的友人以及不少同学都选择了Mac，然而这篇日志并不是想要指导谁或是炫耀什么，目的既是如上所说的记录一下基本配置，也是给大家一些参考，更希望读者能不吝赐教，纠正我的一些因无人指导而独自磕碰出来的不当做法，不管怎么样先谢谢啦~

呐，那就这样开始咯......

# 应用篇

## Sublime Text 3

![](http://pic.ffsky.net/images/2016/03/31/2bfe7d682fa6d54bbdd19ff4328c0c47.png)

主要作战工具。如你所见，在下还是没有壕到免费版能用的情况下还入正

### 安装

提供两种简单方法:
- [官方网站](http://www.sublimetext.com/3)
- homebrew
		$ brew install Caskroom/versions/sublime-text3

### 配置

#### 插件
- Package Control
- Bracket Highlighter
- Ctags
- Side Bar
- LaTeXTools

#### 全局配置文件
直接上传一份至Github比较轻松，主题在用户配置文件中修改，我的是"Flatland Dark.sublime-theme"

### 备注
Sublime对各个插件的使用与支持可能要日后专门开一篇Sublime的日志来详细说明。

尤其是编译命令的编写(如支持编译Opencv)与对LateX的支持

## mpv播放器

![](http://pic.ffsky.net/images/2016/03/31/2b654ba3fe9a546b5c8b6f41c5c475ac.png)

### 安装

懒惰的我这次没有折腾，利用了[前人劳动的成果](http://bbs.feng.com/read-htm-tid-9633783-page-1.html)，在此非常感谢

### 备注

按教程安装后无需任何配置，已经为最终版

## Manico

![](http://pic.ffsky.net/images/2016/03/31/b70b2973694aa8e567532ce45c4db617.png)

图片似乎无法说明功能了，简单来说就是可以自定义app的启动快捷键

[Mac App Store](https://itunes.apple.com/us/app/manico/id724472954?ls=1&mt=12)购买，现在已免费（应该有收费Pro版，在免费之前购买的自动升级为Pro了）

## Yoink

{% youtube zQiU0NkmjZ8 %}

官方短片全面的介绍了这个小应用，请在[官方网站](http://eternalstorms.at/yoink/Yoink_-_Draggings_a_drag_no_more/Yoink_-_Simplify_drag_and_drop_on_your_Mac.html)或[Mac App Store](https://itunes.apple.com/us/app/yoink/id457622435?mt=12)购买应用

## Amphetamine

功能单一却丰富强大，这并不矛盾。它能干的事儿只有阻止Mac自动休眠，但可供调配的参数实在太多了

[Mac App Store](https://itunes.apple.com/us/app/amphetamine/id937984704?mt=12)应该一直是免费的

## Go2Shell

怀念Linux系统下f4呼出当前目录下终端的快捷，Mac要打开一个当前目录的终端无比复杂，于是有了Go2Shell

打开Go2Shell即可获得一个当前目录下的终端，配合Manico使用效果更佳

其实原理非常简单:新建一个终端窗口->cd 当前目录->clear->pwd，

如此简单的原理也直接导致了......它并不是那么好用

[Mac App Store](https://itunes.apple.com/cn/app/go2shell/id445770608?l=en&mt=12)同样免费

## Paste

![](http://pic.ffsky.net/images/2016/03/31/9fd1970f1b0535580fbac09cae325b46.png)
再次怀念Linux，因为Mac是没有原生的剪贴板历史记录的，但是Paste弥补这个遗憾，UI风格也很赞呀~

[Mac App Store](https://itunes.apple.com/app/id967805235?ref=producthunt)

## Hyperdock

如名字所示，是Dock增强软件，它能让你在Dock图标上预览内容，同时还能进行窗口布局管理

### 安装

[官方网站](http://hyperdock.bahoom.com)

### 备注

没有截图的原因是，我已经卸载了。理由是：我在购买后没有收到序列号，发了N封邮件制作者也不理我QAQ

## MenuBar ReArranger 2

真正的好东西！同样如题所示，是用来整理menubar的，它能让你自己排列右上小图标的顺序，当然也能隐藏。

### 安装

[官方网站](http://www.seense.com/mbra/)

### 备注

因为Mac似乎并不允许这种行为，所以听说是自己写的接口......

其实也就是说bug不少：获取当前列表经常错误，建议在自定义中手动加入要排列的app

*另外意外发现隐藏的原理是添加一条超长的占位符，将之后的图标排列到屏幕左侧以外*

# 插件篇

## Aria2

一句话简介：嗯，它是一个下载器~

优点：
- 可以伪装百度云管家...
- 可以伪装迅雷离线（当然还是要会员）...
- 可以伪装...呃，应该没啥还要伪装的了，那最后这个优点就是平时隐身，在终端命令行或者网页界面管理才能看到

缺点:
- 似乎好像是不支持磁力链接解析的，但转成种子就没问题了

### 安装

同样提供两种简单方法:
- [官方网站](https://aria2.github.io)
- homebrew
		$ brew install aria2

### 配置

偷懒的我再次借用了前辈的[劳动成果](/repository/aria2.zip)，再次感谢前辈[雪月秋水君](https://blog.icehoney.me/about))

*请将解压得到的conf配置文件放在~/.aria2目录下(这是一个隐藏文件，没有请新建，并用Shift + Command + G进入)*

在终端中输入

	$ aria2c --conf-path="/Users/xxxxxx/.aria2/aria2.conf" -D

将xxxxxx改为你的用户名(懒惰的我选择写了一个开机自动调用脚本......)

最后，在这个[网页](http://ziahamza.github.io/webui-aria2/)管理你的下载，成功开启aria2后第一次打开网页右上角会弹出Success提示

## Today Scripts

![](http://pic.ffsky.net/images/2016/04/01/00dbc34ede2efec2bdef4e0338d43fdb.png)
这是一款能让你在通知中心运行脚本的App（但我依旧选择将其归类在插件），我并没有编写各种乱七八糟的脚本，[github项目](https://github.com/SamRothCA/Today-Scripts)上有很多作者提供的脚本。

图中是能够查看各种参数的iStats与我自己写的DNS切换

### 安装

网上能搜到的几乎都是只支持Yosemite的版本，github上作者标注的系统也是Yosemite。然而我曾找到过一个修复教程（虽然这会儿找不着了），故在此只能将自用的上传了

[下载](/repository/Today_Scripts.zip)

### 备注

iStats是免费开源软件，安装命令如下

	$ gem install iStats

我就弄错了购买了iStat Menu，结果被过于不与审美相称的UI给吓跑了TAT...

# 碎语篇

其实是结语来着，但似乎能与上面形成闲言碎语的首尾呼应诶~

我的Mac上一些工具性质的、便利自己的配置大致就是这么些，实际上还有一些有趣的小工具并没有列出来（考虑到用得不多）

感谢你能读到这里哦~


