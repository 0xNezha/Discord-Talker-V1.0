# DiscordTalker
Auto send message to Discord Server
Discord Talker V1.0 说明

这是一个很简单的演示脚本，通过调用Discord的API来实现定时向某个频道内发送指定的文本，额外添加了GUI界面，以方便操作，一个实例仅能登录一个账号。（可以复制多份程序到不同的文件夹，以实现“多账号/多频道”发送）
本程序仅供编程学习研究，切勿用于其他用途。如因使用不当造成任何损失，与本程序及作者无关。
程序使用说明：
1、获取Discord账号的登录令牌（即“Token”），可参考该视频：https://www.youtube.com/watch?v=WWHZoa0SxCc

2、获取想要发送信息的频道号码。方法很多，最简单的办法：自己的账号要先加入该Discord服务器，然后点击想要发送信息的频道，在浏览器地址栏内找到最后一段数字即为频道号码。

3、将前两步获取的信息填入配置文件 botConfig.ini 并保存.

4、在talk_list_1.txt 内输入水群信息并保存，每句一行.

5、打开Discord Talker, 点击“启动”即可.


如需打包：

pip install pyinstaller

pyinstaller -F -i favicon.ico discordTalker_GUI.py

在dist文件夹内会生成 discordTalker_GUI.exe ，然后将 botConfig.ini，talk_list_1.txt，logo.png，favicon.ico 拷贝至dist文件夹。 设置完毕后即可双击使用。
