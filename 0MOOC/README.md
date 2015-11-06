# 蟒蛇仙境寻密第一关


目标：创建教程基本框架

所需：gitbook（用于内容呈现），github（用于书的源码托管），disqus（用于读者留言）

步骤：

0. fork 本次课程的仓库到自己的 github 帐号底下

1. 注册 gitbook 帐号，然后创建一个新的图书，接着按照gitbook上面的说明，让自己的gitbook与github用webhooks进行关联，使得你只需要在github上面更新，就可以在gitbook看得到更新后的图书。

2. 这时候我在github更新了一些内容，推送出去，然后到gitbook那里看，发现 build error。仔细一看，原来是我的插件没有配置好。

3. 插件是disqus，找到gitbook官方教程，找到[关于disqus那个页面](https://plugins.gitbook.com/plugin/disqus)，然后按照页面说明进行操作。

4. gitbook官方文档告诉我：creating a new website on the disqus.com website，这个完全不知道是什么回事（汗颜，之前没有用过disqus），就直接扔到google去搜，原来，disqus官方也有[文档说明](http://disqus.com/admin/signup/)呢。当然，首先还是要先有个disqus帐号。

5. 于是，创建了disqus项目，有了个shortname，然后把这个shortname填到gitbook代码仓库根目录的 book.json 那里（此处假如担心修改后的文件语法有误，可以到 [JSONlint](http://jsonlint.com/) 那里去检查是否有语法问题），再 git add && git commit && git push，也就成事了。

6. 回到 gitbook 图书页面，应该可以看得到像模像样的私人python教程咯。