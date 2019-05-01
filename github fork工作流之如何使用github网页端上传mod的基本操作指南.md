github操作指南之如何在网页端上传mod
这篇介绍：如何用github网页端上传cataclysmdda的mod到Mod分享平台。

ps：除了网页端操作之外，还可以用github desktop或TortoiseGit 或git操作。尤其是一次性大批量对多个文件内容进行修改上传且一起提交的时候，使用软件会更便捷高效。这里就不作详细介绍了。

1、首先要注册一个github帐号，如已有帐号则请登录。
2、用浏览器打开https://github.com/cddamods/cddamods.github.io，如图1点击fork，把这个项目仓库的副本复制到自己帐号里。
 
![图1](https://upload-images.jianshu.io/upload_images/7643202-e011e66301c17649.gif?imageMogr2/auto-orient/strip)

 
图2

Fork后回到仓库就能看到自己fork的项目，并可以看到项目是从哪个仓库fork来的。
 
图3

Ps：图3显示的3，表示已经有3个人fork了这个项目。


 
图4 主要按钮翻译
 
图5
3、如图5，创建新的分支，名称可随意，这里我创建了upload分支。
4、在upload分支的cddamods.github.io/cn/mods里点击 upload files 上传文件。
 
图6
如图6，把mod压缩包拖到上图位置或者点choose your flies 手动选择文件。
 
图7
如图7，在Commit changes里输入说明，确定。压缩包上传完成。
5、直接在浏览器打开upload分支的cddamods.github.io/cn的modsinfo.json.
 
图8
如图8点击铅笔按钮，开始在浏览器里编辑modsinfo.json。按照readme.md的格式说明，参照已有内容，补充修改要增加的mod的介绍文字。

 
图9
如图9编辑好后，同样如图7那样在Commit changes里输入说明，确定。

 
图10
6、如图10，现在，点击上图的按钮，把upload分支与原项目（cddamods/cddamods.github.io的master分支）进行比较并推送到cddamods/cddamods.github.io。
 
图11
如图11，再次输入说明，确定。
 图12
如图12，系统自动判断与原项目是否有冲突，绿√表示没有冲突。
---------------------------------
等项目作者或管理员审阅，如果审核通过，会将你提交的内容合并到master主分支。
一旦项目作者或管理员审核通过，你提交的内容就合并更新到cddamods/cddamods.github.io的master主分支。这样，mod上传就正式完成了。

-------------------------
假设过了几天，你又想上传其他mod，而作者与其余贡献者已经对这个项目又做了一些修改。
为了避免冲突，那你最好在他们的修改的基础上"同步你的fork"，还要再做一些修改！
"同步你的fork"有3种方法：
方法1：直接在网页端删除你fork的项目，再重新fork。(这无疑是最暴力有效省事的方式。)删除操作如下面3张图：
 
 
 

方法2：使用网页端手动更新你fork的项目从cddamods/cddamods.github.io的master主分支同步更新到自己帐号/cddamods.github.io的master主分支，以确保在最新的复制版本里工作。（对于新手来说容易弄错，不推荐）
同步更新具体操作情况请参考以下网页内容：
github fork 别人的项目源作者更新后如何同步更新 - zhongzunfa的专栏 - CSDN博客，https://blog.csdn.net/zhongzunfa/article/details/80344585

并且建议另建一个新分支进行修改操作，之前的旧分支upload可以删掉了。
参考以下网页内容：GitHub网页版删除分支 - yanhanhui1的博客 - CSDN博客 ， https://blog.csdn.net/yanhanhui1/article/details/82819665

方法3：使用git命令行同步你fork的项目，需要安装git。
参考github笔记一：保持fork之后的项目和上游同步 - 简书
https://www.jianshu.com/p/43dfe8d59b70


