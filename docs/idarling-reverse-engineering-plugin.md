# IDArling:IDA Pro 和 Hex-Ray 的协作逆向工程插件

> 原文：<https://kalilinuxtutorials.com/idarling-reverse-engineering-plugin/>

IDArling 是一个针对 [IDA Pro](https://www.hex-rays.com/products/ida/) 和[Hex-ray](https://www.hex-rays.com/products/decompiler/index.shtml)的协同逆向工程插件。通过将 IDA Pro 的不同实例连接在一起，它允许实时同步多个用户对数据库所做的更改。

IDArling 的主要特点是:

*   挂钩一般用户事件
*   结构和枚举支持
*   十六进制射线反编译器同步
*   重放引擎和自动保存
*   数据库加载和保存
*   交互式状态栏小部件
*   用户光标(指令、功能、导航条)
*   邀请并跟随用户移动
*   使用 Qt5 的专用服务器
*   IDA 内的集成服务器
*   局域网服务器发现
*   实时跟踪用户的移动

如果您有任何不值得报告的问题，请随时通过 freenode 上的 [#idarling 联系我们并提出问题。](https://kiwiirc.com/client/irc.freenode.net/idarling)

**也读作-[Frida extract:基于 Frida.re 的 RunPE 提取工具](https://kalilinuxtutorials.com/fridaextract/)**

**发布**

这个项目正在积极开发中。如果你想帮忙的话，请随时发送一份公关！🙂

它目前的状态并不稳定，请继续关注该项目的第一次发布！

**安装**

将 IDArling 客户端安装到 IDA 插件文件夹中。

*   将`**idarling_plugin.py**`和`**idarling**`文件夹复制到 IDA 插件文件夹。
    *   在 Windows 上，该文件夹位于`**C:\Program Files\IDA 7.x\plugins**`
    *   在 macOS 上，该文件夹位于`**/Applications/IDA\ Pro\ 7.x/idabin/plugins**`
    *   在 Linux 上，该文件夹可能位于`**~/ida-7.x/plugins/**`
*   或者，您可以通过将以下行复制到控制台来使用“简易安装”方法:

**导入 urllib2exec(URL lib 2 . urlopen(' https://raw . githubusercontent . com/IDArlingTeam/IDArling/master/easy _ install . py '))。read()**

**警告:**该插件仅与 Windows、macOS 和 Linux 上的 IDA Pro 7.x 兼容。

专用服务器需要集成到 IDA 中的 PyQt5。如果您使用外部 Python 安装，我们推荐使用 Python 3，它提供了一个预构建的包，可以通过简单的`**pip install PyQt5**` **进行安装。**

**用途**

打开*设置*对话框，可通过右键单击状态栏中的微件打开。点击*网络设置*选项卡显示服务器列表，并将您的服务器添加到列表中。

再次右键单击小部件后，通过单击连接到服务器。最后，您应该能够访问以下菜单来上传或下载数据库:

**文件—>从服务器打开
文件—>保存到服务器**

**信用:Alexandre Adamski &乔佛里·吉本**

[**Download**](https://github.com/IDArlingTeam/IDArling)