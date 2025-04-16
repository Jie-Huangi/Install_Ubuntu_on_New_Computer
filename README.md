# Install Ubuntu on New Computer
 
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

> 现在有了新的发现。经过测试发现，搜狗输入法在我的Ubuntu 22.04 上不能用的根本原因是Chrome内核太高了。当我的内核降低为134.xxxx的时候，搜狗输入法是可以正常运行。
> 所有的问题都出现在Chrome内核浏览器上，其他地方搜狗输入法可以正常使用。

## chrome 浏览器降低内核

> 卸载浏览器
> sudo apt remove google-chrome-stable   # remove/ purge
> sudo apt purge google-chrome-stable    # 卸载更加干净


[chrome浏览器旧版本网址](https://www.slimjet.com/chrome/google-chrome-old-version.php)

[edge浏览器旧版本网址](https://packages.microsoft.com/repos/edge/pool/main/m/microsoft-edge-stable/)

cd ~/Downloads
sudo dpkg -i google-chrome-stable_OLD_VERSION_amd64.deb

sudo apt --fix-broken install


> 禁止升级 chrome and edge
> sudo apt-mark hold google-chrome-stable

> sudo apt-mark hold microsoft-edge-stable

> 解除升级 command
> sudo apt-mark unhold google-chrome-stable

> sudo apt-mark unhold microsoft-edge-stable



## ubuntu 向日葵闪退

https://blog.csdn.net/m0_46259216/article/details/121513562

## ubuntu 截图工具

<https://blog.csdn.net/sexyluna/article/details/105884224>

## linux 软件推荐

<https://alim0x.gitbooks.io/awesome-linux-software-zh_cn/content/>


## zotero中文社区

https://zotero-chinese.com/user-guide/plugins/zotero-gpt.html

