# 模板名称Me

>模板名称 Me
>
>主题名称 Knowledge Brain
>
>订阅推荐码：X0sndna 感觉不错，订阅思源的时候可以支持一下，早买早享受！
>
>思源官网：https://b3log.org/siyuan/
>
>思源社区：https://ld246.com/domain/siyuan

### 模板介绍

1. 模板早期是在Meteor的基础进行添加修改的
2. 花费一些时间去看 sprig 的函数，这些模板修改还是花费了很多时间
3. 应该有很多人自己添加修改模板 ，只是没有选择分享出来
4. 希望多一些分享，发扬下人人为我，我为人人的精神

### 12月29日

1. 因为思源更新1.55需要修改readme.md文件的名称特此更新

### 11月3号更新

1. 修改了下daily note改为我自己喜欢用的那种样式
2. 因为我不怎么使用模版，集市上也没感觉有几个人用，没有更新的动力

### 8月22号更新

添加doc-list-child5 只展示一层子目录，孙子目录不展示

### 8月21号更新

1. 模板所有path改为hpath
2. 添加doc-list-child1 列出该文件所有的子文件目录的双链
3. 添加do-list-child2 列出该文件所有的子文件目录的双链
4. 添加do-list-child3 列出该文件所有的子文件目录的双链
5. child123展示效果略有不同,按照字母生序排列

### 8月19号更新

在Info_Catalogue.md的模板的基础修改添加了两个目录模板doc-list、doc-list-folder

列出当前文件及其子文件夹下所有的笔记的双链引用

排序方式按照字母或者数字递增自然顺序排序

两种的区别如下

1. doc-list 会显示第一层文件夹名称
2. doc-list-folder 不会显示第一层文件夹名称
3. 效果图如下

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210819213503-yduakq8.png)

### 8月8号更新

1. 修改了live2dm1为live2d-m1
2. 添加了live2d-m3为网易云轻音乐[歌单地址](https://music.163.com/#/my/m/music/playlist?id=368529707)：https://music.163.com/#/my/m/music/playlist?id=368529707

### 8月5号更新内容

首恭喜中国乒乓女团夺得冠军 🏆，香港女团夺得季军

1. 模板添加了live2d系列3个

2. 具体请看下面的live2d介绍

3. 在dailynote那个模板上添加了日记快捷方式操作

#### Live Second Dimension（live2d）介绍

这次更新的内容分别是 live2d 、live2d-m1、live2d-m2

live2d 是动态的二次元人物

live2d-m1（漏了个-）则是在 live2d 的基础上添加了 音乐播放，目前的歌单是我的一个网易云音乐歌单，等以后思源有了 widget 应该可以自定义歌单

live2d-m2 是在 live2d 的基础上添加了一个第三方的音乐 H5 播放器，可以自己选择歌单，但是缺点明显 **免费用户只能有一个显示音乐播放器**

#### live2d

> 这个是在 https://github.com/stevenjoezhang/live2d-widget 的基础上修改了一点点内容
>
> 放在我的云服务器里，加载速度不是很快
>

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210805173138-eprrbki.png)

#### live2d-m1

> 播放器的内容来自我网易云音乐的歌单https://music.163.com/#/playlist?id=606641571
>
> 源码来自 https://github.com/metowolf/MetingJS#quick-start 可以自己定制
>
> 因为网速的原因一些内容加载过慢显示错误，不影响使用
>

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210805173051-a410zqe.png)

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210805173106-3ssmv1x.png)

#### live2d-m2

> 这是播放器是第三方 https://myhkw.cn/提供的
>
> 免费用户限制 ip
>
> **一个 ip 播放器只会显示一个，即使多个页面添加**
>
> 即使建立多个页面或者 iframe 也是只有一个页面会显示播放器
>

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210805173347-wh6s940.png)

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210805173255-bymh0jk.png)

### 7月4日模板初次添加

#### 修改内容介绍

1. 修改模板名称原先的是 Meteor 有点长，改成了 Me
2. 修改了每一个模板命名，原有的每次都不知道什么意思，现在的见名知意
3. 修改了 dailynote，原有的太臃肿了，现在的只有一张图片，一个提示，一个时间
4. 修改了随机图片个数，原有的 32 张，**现在的是 234 张**包含原有的且多为 4K8K，[图片地址](https://github.com/LaneDu/SiYuan/tree/main/pic) 存在在我的 GitHub 上，可能加载有些慢，个人感觉还可以，有好的图片也可提 issues，发网盘链接，我添加进去
5. dailynote-mypic 和 dailynote-oldpic 分别代表我的 234 张和原来的 32 张，dailynote 原有的没变
6. doc-list 是按照 文档名称查询包含文档名称文件夹下的所有文档列表
7. todo-list 我改成了 todo doing done 的形式，原有的样式也保留了
8. 添加了一个 todo-daily，也是一张图片，一个时间，一个 todo list

#### 图片展示

**dailynote-mypic**

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210706110408-ohn80ml.png)

**todo-daily**

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210706110520-qnwa9mr.png)

**doc-list**

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210706110721-vvfizzt.png)

**类型一览**

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210706110239-3m2oj0d.png)

**日记本设置**

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210706111135-lt1nmvb.png)



