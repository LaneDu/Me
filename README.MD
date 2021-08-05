### 8月5号更新内容

1、主题代码行号改为固定大小

2、去掉了iframe的边界线

3、模板添加了live2d系列3个

4、等思源的组件出来之后，估计用户可以自定义歌单

### Live Second Dimension（live2d）介绍

#### live2d

> 这个是在 https://github.com/stevenjoezhang/live2d-widget 的基础上修改了一点点内容
>
> 放在我的云服务器里，加载速度不是很快
>

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210805173138-eprrbki.png)

#### live2dm1

> 播放器的内容来自我网易云音乐的歌单 https://music.163.com/#/my/m/music/playlist?id=2235447397
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

### 模板名称 Me

#### 简单介绍

1. 把两个已有的模板整合成了一个，说抄袭也可以哦，我没有任何收益的，只是想分享一下
2. 我不会 go 也没时间去看 spring 的函数，没有做太大的改动，但是改动依然花费了大半天时间
3. 保留了原有的功能，如果原先模板的不添加新功能，那么可以删掉原有的那两个
4. 我算是才刚开始用，应该有很多自己修改模板的人 ，更好的模板只是没有选择分享出来
5. 希望多一些分享，发扬下人人为我，我为人人的精神

#### 修改内容

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

### 主题名称 Tsundoku change

#### 简单介绍

1. 先吐槽下这个日语名字 Tsundoku，发音和意思真的难
2. 根据名字也知道，这是在思源刚更新 1.2 版本的时候，原先的模板样式没了，这个 Tsundoku 不错
3. 根据 Tsundoku light 修改的，这次顺便一起提到了集市
4. 如果以后再更新，可能会改个名字
5. 我现在比较喜欢的主题有 [Sci-Fi](https://github.com/VIWZ/Sci-Fi)、Room、Wave、Tsundoku
6. Tsundoku 十分流畅，Sci-Fi 主题特别炫酷，可是太卡了，难以使用，向作者提了 issues，不知道能否优化下

#### 修改内容

1. 标题颜色
2. 引用颜色
3. 代码块背景
4. 标签颜色
5. 等等

#### 图片展示

![image.png](https://b3logfile.com/siyuan/1619927307428/assets/image-20210706112905-h93nlox.png)

### 结语

现在可以去集市上下载体验下了

模板名称 Me

主题名称 Tsundoku Change

订阅推荐码：X0sndna 有需要的可以支持一下思源，早买早享受！

思源官网：https://b3log.org/siyuan/

思源社区：https://ld246.com/domain/siyuan
