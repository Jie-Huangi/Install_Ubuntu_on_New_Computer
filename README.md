1、系统安装

2、换源

3、打开代理

4、显卡驱动

5、常用软件安装

## 输入法

[Ubuntu 22.04安装搜狗输入法](https://blog.csdn.net/Mr_Sudo/article/details/124874239)

> 遇到的一些问题
> 直接安装的 sudo apt install fcitx5 和 sudo apt install fcitx5-chinese-addons
> 使用里面自带的pinyin输入法。
> 如果要使用sougou输入法，必须安装 fcitx4 才可以匹配搜狗程序，否则会报错。
> 最开始安装的就是搜狗，也是fcitx4 但是不知道什么原因，浏览器里面不能使用搜狗输入法了。
> 后面在闲鱼上面找技术，安装了fcitx5，勉强能用。
> fcitx5面临的问题是在chrome浏览器中输入文字的时候会挡住输入框中的文字，后面经过多次尝试，我发现只需要改变浏览器页面的位置，输入法的边界框也会跟着移动，这样，打字的时候就不会挡住我输入的内容。算是可以正常使用了。

## ubuntu 截图工具

<https://blog.csdn.net/sexyluna/article/details/105884224>

## linux 软件推荐

<https://alim0x.gitbooks.io/awesome-linux-software-zh_cn/content/>


## zotero中文社区

https://zotero-chinese.com/user-guide/plugins/zotero-gpt.html


## chrome 浏览器降低内核

> 卸载浏览器
> sudo apt remove google-chrome-stable   # remove/ purge
> sudo apt purge google-chrome-stable    # 卸载更加干净


[chrome浏览器旧版本网址](https://www.slimjet.com/chrome/google-chrome-old-version.php)


cd ~/Downloads
sudo dpkg -i google-chrome-stable_OLD_VERSION_amd64.deb

sudo apt --fix-broken install


> 禁止升级 chrome and edge
> sudo apt-mark hold google-chrome-stable
> sudo apt-mark hold microsoft-edge-stable

> 解除升级 command
> sudo apt-mark unhold google-chrome-stable
> sudo apt-mark unhold microsoft-edge-stable


# edge 旧版浏览器

[edge浏览器旧版本网址](https://packages.microsoft.com/repos/edge/pool/main/m/microsoft-edge-stable/)

## ubuntu 向日葵闪退

https://blog.csdn.net/m0_46259216/article/details/121513562

## edge 浏览器 侧边栏问题

我是在windows 和Linux系统下同事出现不可用的问题。

>windows下面是当时出现的情况是可以打开copilot，但是给copilot发消息，不给我答案，报错，说什么网络出现异常等等，服务器繁忙之类的问题。
我自己试着改了一下，更改浏览器的地区、语言之类的，也去看了相关的视频，但是没有解决我问题。

后面去咸鱼找了技术，花了35块钱。

技术上来就给我浏览器清除了历史记录和cookie之类的东西。我当时惊呆了，我四年的数据，一秒就没了。没拦住事情已经发生了。

接着他是又给我浏览器添加了一个账号。后面据他说，账号是之前买的。

更新了一个账号过后，再去点击copilot还是没有反应。

后面他发现我copilot的图标和最新版的图标不一样，就问我是不是没有更新软件。我说是的。

他一顿操作，就给我更新了软件。

更新完过后，copilot就可以使用了。

35块钱就这样没了。

等他下线我切换回了自己的账号，copilot照样能用。

可恶，问题的根源在于我没有更新软件。


晚上，我又自己倒腾了一下Linux系统。

我是在gork3上面搜的解决方法。我的描述语是

> edge 浏览器，ctrl + shift +/呼喊出来的侧边栏，出来侧边栏了，但是里面的图标不能点击，点击了没有反应

给我生成一堆答案，我看到一个让我先将浏览器内核，降到126，再升级到134，问题就可以解决。

我照做了，问题得到解决。

> 这两天一直在弄电脑问题，主要集中在输入法和copilot侧边栏上面。
输入法主要是chrome内核的浏览器不能太新，不然浏览器无法切换页面
copilot的问题在win上面应该就是需要升级到最新版，同时打开外网，就可以正常使用，问题应该没有那么复杂
在Linux上面，解决问题的关键应该是先降到126内核，在升级到134内核就可以。问题根源可能是安装包里面有些依赖没有吧！


