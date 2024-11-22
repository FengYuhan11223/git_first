git使用问题记录



1、Q：无法克隆别人的项目

![](https://i-blog.csdnimg.cn/blog_migrate/53c32e4bf4086f0eb87077dcb62f76b5.png)

       A：并非是因为推文所说的没有翻墙，而是因为没有在github中添加公钥

[github 公钥产生和配置_github公玥-CSDN博客](https://blog.csdn.net/wslyk606/article/details/80779608)

Q：在配置过程中由于我C盘中.ssh上级的文件是中文，我无法在git bash中使用生成公钥和私钥的命令

       我的解决方法：打开命令运行框，在windows运行窗口实现生成公、私钥进行配置不知可行否，最后运行倒是可以但是无法确定这样操作是否安全T_T

        网上的解决方法是将git bash中的文字识别添加utf-8，但我的电脑使用后依旧中文乱码。



2、Q：无法连接远程仓库—>fatal: unable to access ‘https://github.com/.../.git‘

      A：[完美解决 git 报错 “fatal: unable to access ‘https://github.com/.../.git‘: Recv failure Connection was rese-CSDN博客](https://blog.csdn.net/qq_43546721/article/details/139506583)

       P.S.:最开始尝试方法一未成功，再采用方法二也未成功，并且端口变成了代理服务器的端口，于是又用方法一的代码取消了代理设置，再次连接仓库，成功了。



3、Q：连接远程仓库后，无法同步本地库与远程库，push失败

      报错信息一：fatal: Not a git repository (or any of the parent directories): .git

      A1：输入git init

            [解决 fatal: Not a git repository (or any of the parent directories): .git 问题-CSDN博客](https://blog.csdn.net/wenb1bai/article/details/89363588)

       报错信息二：error: failed to push some refs to 'https://github.com/...

        A2：输入git push -u origin master -f（即链接中的方法三、打的代码最少的那个...）

        [[如何解决error: failed to push some refs to ‘git@github.com:......git pull冲突问题-CSDN博客](https://blog.csdn.net/weixin_43922901/article/details/89426923)

        注：我使用教程中的步骤到这步报错时，用[解决办法：git错误 error: failed to push some refs to 'https://github.com/..._failed to push some refs to 地址-CSDN博客](https://blog.csdn.net/dietime1943/article/details/85682688)的方法没用



此外还遇到过以下两种报错（附解决方法）：

[Git报错解决：fatal: unable to access ‘https://github.com/...‘: OpenSSL SSL_read:..., errno 10054-CSDN博客](https://blog.csdn.net/ME_GIRL/article/details/118572491)

[git clone出现 fatal: unable to access 'https://github.com/...'的解决办法(亲测有效)-CSDN博客](https://blog.csdn.net/Dashi_Lu/article/details/89641778)






