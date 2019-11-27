# rime鼠须管

## 安装方法

### 稳定版下载

官方最近终于更新版本，之前一直14年版本，有点太老了。官方已经更新到[0.14.0 (2019-06-23)](https://bintray.com/rime/squirrel/release), 可以直接官方下载安装。

### 最新版本下载

如果想尝试最新功能，可以下载squirrel测试版本 <https://bintray.com/rime/squirrel/testing/0.14.0%2Bgit08ed4f4>。最近新加了`vim_mode`功能，我就下载了最新版本。

### 编译安装

想自己修改一些功能的，或者使用最最新的功能，可以自己编译安装。具体的编译方法如下:

``` bash
#安装Xcode的工具,运行下面的命令

xcode-select --install

# 使用 [Homebrew](http://brew.sh/)安装相差依赖库:
# dev tools:
brew install cmake
brew install git
# libraries:
brew install boost

#下载源代码
git clone --recursive https://github.com/rime/squirrel.git

cd squirrel

#编译依赖库
make deps

#编译squirrel
make

#安装squirrel
sudo make install
```

## 配置

1. 打开用户设定, 找到用户配置文件夹。

    ![config](https://beyondkmp.com/imgs/rime/config.png)
2. 将之前的用户配置删除，然后将此git的内容下载到用户配置目录下。
3. 重新加载就大功告成了。

    ![reset](https://beyondkmp.com/imgs/rime/reset.png)


