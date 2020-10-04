

## 1.Python 下载与安装

Python 2.7的终止日期最初定为2015年，由于担心大量现有代码无法轻易地移植到Python 3而推迟到2020年，Python3.X在库的名称上也有所改变，所以建议安装Python3.X版本。这里以win7 64位笔记本为例：

**1.1官网下载**

[python官网地址](https://www.python.org/downloads/windows/)

打开上面官网链接地址，找到目前最新stable版本，点击红色箭头链接

![](images/python1.png)

进入下图所示网页

![](images\python0.png)

滑动滚动条，找到如下图箭头所示

![](images\win64download.png)

下载安装包后直接以管理员身份运行（注意勾选图中箭头所示选项！！！）

![](images\python3.png)

![](images\python4.png)

安装完成后，打开cmd命令窗口，输入python,出现下图所示内容即安装python成功！

![](images\cmd.png)

![](images\cmd-python.png)

## 2.配置python pip国内源

2.1新建 pip 配置文件夹，直接在user用户目录中创建一个名为 pip 的文件夹( 即%HOMEPATH%\pip)，如下图所示：
![](images\pip1.png)

接着在 pip 文件夹中创建一个名为 pip 的文本文件(后缀名由" .txt "改为 " .ini ")，格式如上图所示：

 文件内容如下：

```
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
[install]
trusted-host = https://pypi.tuna.tsinghua.edu.cn
```

修改完成后**保存**，启动cmd，使用 " pip install xxx "(xxx为你要下载的包名，比如 pip install numpy)，即可默认使用国内源下载。

## 3.Visual Studio code(VS code)下载与安装

官网下载

[VS code官方网址](https://code.visualstudio.com/Download)

选择**System Installer**版本下载，如下图所示

![](images\0.png)

安装包下载后右键以管理员身份运行

勾选同意，点击下一步

![](images\2.png)

修改或默认安装目录，点击下一步

![](images\3.png)

一直点击下一步，直到完成安装就行

![](images\5.png)

![](images\6.png)

## 4.VS code 简单配置与简单使用

首先打开VSCode软件，可以看到刚刚安装的VSCode软件默认使用的是英文语言环境，如下图：

![](images\vs_1.png)

这里需要使用快捷键【Ctrl+Shift+P】来实现，如下图：

在弹出的搜索框中输入【configure language】，然后选择搜索出来的【Configure Display Language】,如下图：

![](images\vs_2.png)

点击后，可以看到旁边**EXTENSIONS: MARKETPLACE** 中有多种语言可以选择，你只要选择中文，进行安装，然后安装完成会重启软件，然后打开就是中文的了。



![](images\vs_3.png)

同样地，在扩展商店EXTENSIONS: MARKETPLACE(扩展：商店)中安装python插件，如下图所示，重启VS code

![](images\vs_6.png)

使用快捷键【Ctrl+N】新建文件，并保存为hello.py(后缀名不能省)

输入

```
print("python")
```

快捷键【Ctrl+S】保存即可，打开终端（如下图所示），点击Run按钮，可看到终端输出内容。

![](images\vs_7.png)

## 5.Jupyter notebook安装

在上图demo目录（目录下有hello.py Untitled-1.py 等文件）下打开cmd，命令行输入

**pip install jupyter** 即可安装jupyter notebook

等一会儿，直接在命令行输入**jupyter notebook**

笔记本默认浏览器就会自动打开页面

![](images\jupyter1.png)

