
# Grasscutter2.8.52
这个仓库会收集更新已知的代码，来实现测试Grasscutter2.8到Grasscutter3.0升级。发现问题可以向我报告（如果可以请用简体中文，谢谢）。<br>

## 目前实现功能：
1.行纪正常领奖<br>
2.大世界部分宝箱可通过解迷开启。<br>
3.新增须弥角色(可放卡池)、命星道具。<br>
4.新增须弥怪物、武器、突破材料（加入合成台）。<br>
5.他内容同2.8版一样<br>
## 如何运行它？
必备环境：
Java17 与 MongoDB (recommended 4.0+)

在开始之前，你需要下载它<br>
https://download.oracle.com/java/17/archive/jdk-17.0.3.1_windows-x64_bin.exe<br>
https://www.mongodb.com/try/download/compass<br>
https://www.mongodb.com/try/download/community<br>

## 服务设置
（资源文件我不会经常去更新它，请到这里下载）<br>
1.下载GC3.0版本:https://github.com/lassedds/3.0-GC/releases/tag/Release

2.下载资源文件:https://github.com/lassedds/3.0-Resources

3.将资源文件放入3.0GC文件夹中并命名为"resources"。

4.右键单击start_config.cmd文件，然后选择**编辑**。接下来，你必须在你安装的java版本的文件夹中找到 "*bin*" 文件夹。它应该在 **`C:\Program Files\Java\`**, 在此路径下打开 "*jdk-17.x.x.x*" 文件夹，然后打开 "*bin*" 文件夹并复制文件路径。类似这样: **`C:\Program Files\Java\jdk-17.x.x.x\bin\`**。  把它放进你的 *start_config.cmd* 文件作为变量 "*JAVA_PATH=*"。

5:你现在可以使用*start .bat*文件来开启服务。

6:打开你电脑上的3.0 Genshin文件夹，并把<a href="https://drive.google.com/file/d/1esXUB4Q_Y_wDjvqnNbN8jiQUKsO11N1S/view?usp=sharing">该文件</a>放在在这两个位置:<br>
1. "*YOURGENSHINFOLDER/GenshinImpact _ Data/Managed/Metadata*"<br>
2. "*YOURGENSHINFOLDER/GenshinImpact _ Data/Native/Data/Metadata*"

## Fiddler 代理

1.从<a href=https://www.telerik.com/download/fiddler>这里</a>下载Fiddler Classic。

2.打开Fiddler Classic后，在软件窗口顶部找到**Tools**选项，然后选择**Options**。

3.在**Options**菜单中你会看到很多子菜单，选择**HTTPS**子菜单，然后单击文本旁边的小方框**Decrypt HTTPS traffic**。

4.完成第3步后，选择选项菜单下的**Connections**子菜单。然后选择**Fiddler Classiclistens onport**选项，默认情况下，端口为'8888'。你也可以单击**change**来使用其他的端口，比如我用的是8080。

5.在选项菜单中选择**OK**并单击**FiddlerScript**按钮。然后<a href=https://github.lunatic.moe/fiddlerscript>从这里</a>找到脚本文件，复制脚本代码。回到Fiddler，用刚才复制的脚本替换现有脚本，然后单击**Save Script**按钮。

6.现在你可以启动游戏了，但是你还没有完全完成。在你尝试登录时，Fiddler中会弹出一些菜单，全部选择确认即可。

7.成功！现在你应该已经设置好Fiddler了。如果您有任何问题，欢迎加入我们的<a href=https://discord.gg/AYtB7Q2er8>Discord</a>


## 客户端支持：
内测端2.850、内测端2.851、内测端2.852（推荐）

## 常见问题
###### 开门白屏：确认客户端补有没有替换、数据库被破坏（建议删库重来）、客端被破坏，通常是因为开挂（重启电脑可解决）

###### 连接超时：确认客户端代理是否正常？

###### 提示4124：确认客户端补有没有替换？

###### 打开客户端闪退：重启电脑没解决，安装c++运行库
