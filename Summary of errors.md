# Errors QAQ



## Q1:AttributeError: module 'gym.envs.box2d' has no attribute 'BipedalWalker'
> https://blog.csdn.net/weixin_43729393/article/details/89423946

总结：需要安装box2d

## Q2:pytorch和torchvision

一开始不会装pytorch，后来发现https://pytorch.org/ 写的很详细。

## Q3:gym.make() Atari游戏失败

重装gym[atari]模块

> 原文 https://github.com/openai/gym/issues/1726
>
> 翻译版 https://blog.csdn.net/weixin_44210881/article/details/103031995

这个问题遇到过两次……第一次通过

> pip install --no-index -f https://github.com/Kojoley/atari-py/releases atari_py

就解决了，然而第二次这样就失败……然后根据上面的链接似乎解决了，说似乎是因为……我还是没有把整个代码跑完就又出了新的错QAQ……如果还有问题下次补充。

## Q4: windows 10 安装mujoco模块

> https://zhuanlan.zhihu.com/p/92578711
>
> https://zhuanlan.zhihu.com/p/104178775

按照以上方法我在我的环境上安装成功mujoco了，但是gym的版本真的是有点虐，跟新版在某些参数上有出入，然后就会发现新的问题……~~所以因为我自己毕业设计环境要自己写可能还是会用更新的版本，加上下面那条，我真的开始时不时思考要不要买个mac。 什么，linux双系统（or 虚拟环境）？那就更多泪了……~~

## Q5: windows 10 安装universe

我只是看到一本书上面可以训练机器人在旷野上奔跑的图就心动不已非要试试……由于一直搞不懂Docker怎么用而失败，下面是我找到的看起来比较完善的教程，欢迎能够实操的小伙伴前来讨论（教教我）。

> https://www.jianshu.com/p/536d300a397e

## Q6: seaborn 画图 没有阴影的置信区间

好了起因又是我看人家论文里面的图很酷炫想画一个，譬如

![1587028313841](https://github.com/drarryon/Deep-Reinforcement-Learning/blob/master/laji/1587028313841.png)

来自https://arxiv.org/abs/1802.09477v1

然后我兴冲冲地下载了大佬的代码然后开始跑……大佬只给了算法代码（~~白嫖画图代码失败~~）……然后就开始百度如何绘制这样的曲线，了解到可以用seaborn，然后找到教程，load刚用大佬的代码跑出来的数据，并没有那种酷炫的效果。原因是数据的time是唯一的，并没有置信区间，需要增加更多行。这个问题是男朋友在看了官方给的数据样例想到的，赞美他！以下是我们画出来的效果，蓝色是大佬的结果（~~多么希望我的算法也可以快点跑出来这样的曲线~~），橘色是随机生成的数。

![1587028773507](https://github.com/drarryon/Deep-Reinforcement-Learning/blob/master/laji/1587028773507.png)

未完待续……（真的不想再看到error了QAQ）

# 致谢

最后，非常感谢提供了解决方法的作者大佬们。给你们鞠躬了！
