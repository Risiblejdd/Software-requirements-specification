# 软件需求说明书 for OCMP

## 一、引言

### 1. 1 目的

​	为明确软件需求、规划项目、确认进度、组织软件开发并测试而撰写本文档。同时，详细分析项目总体需求，可以作为软件开发工作的基础和依据以及确认测试和验收的依据。

### 1. 2 背景

​	本次开发的项目为线上共享听歌聊天平台，由团队Tom & Jerry提出并开发。

### 1. 3 定义

| 序号 |    缩写    |                             定义                             |
| ---- | :--------: | :----------------------------------------------------------: |
| 1    |    IDEA    | IDEA 全称 IntelliJ IDEA，是Java编程语言开发的集成环境。IntelliJ在业界被公认为最好的Java开发工具，尤其在智能代码助手、代码自动提示、重构、JavaEE支持、各类版本工具(git、svn等)、JUnit、CVS整合、代码分析、 创新的GUI设计等方面的功能可以说是超常的。IDEA是[JetBrains](https://baike.baidu.com/item/JetBrains)公司的产品 |
| 2    |   chrome   | Google Chrome是一款由[Google](https://baike.baidu.com/item/Google)公司开发的网页浏览器，该浏览器基于其他[开源软件](https://baike.baidu.com/item/开源软件/8105369)撰写，包括[WebKit](https://baike.baidu.com/item/WebKit)，目标是提升稳定性、速度和安全性，并创造出简单且有效率的使用者界面。 |
| 3    |    Java    | Java是一门[面向对象](https://baike.baidu.com/item/面向对象)编程语言，不仅吸收了[C++](https://baike.baidu.com/item/C%2B%2B)语言的各种优点，还摒弃了C++里难以理解的[多继承](https://baike.baidu.com/item/多继承)、[指针](https://baike.baidu.com/item/指针/2878304)等概念，因此Java语言具有功能强大和简单易用两个特征。 |
| 4    | JavaScript | JavaScript（简称“JS”） 是一种具有[函数](https://baike.baidu.com/item/函数/301912)优先的[轻量级](https://baike.baidu.com/item/轻量级/22359343)，解释型或即时编译型的高级[编程语言](https://baike.baidu.com/item/编程语言/9845131)。虽然它是作为开发Web页面的[脚本语言](https://baike.baidu.com/item/脚本语言/1379708)而出名的，但是它也被用到了很多非浏览器环境中，JavaScript 基于原型[编程](https://baike.baidu.com/item/编程/139828)、多范式的动态脚本语言，并且支持[面向对象](https://baike.baidu.com/item/面向对象/2262089)、命令式和声明式（如[函数式编程](https://baike.baidu.com/item/函数式编程/4035031)）风格 |
| 5    |    HTML    | HTML称为[超文本](https://baike.baidu.com/item/超文本/2832422)标记语言，是一种标识性的语言。它包括一系列标签．通过这些标签可以将网络上的文档格式统一，使分散的[Internet](https://baike.baidu.com/item/Internet/272794)资源连接为一个逻辑整体。HTML文本是由HTML命令组成的描述性文本，HTML命令可以说明[文字](https://baike.baidu.com/item/文字/612910)，[图形](https://baike.baidu.com/item/图形/773307)、[动画](https://baike.baidu.com/item/动画/206564)、[声音](https://baike.baidu.com/item/声音/33686)、[表格](https://baike.baidu.com/item/表格/3371820)、[链接](https://baike.baidu.com/item/链接/2665501)等 |
| 6    |    OMCP    |                线上听歌聊天平台（本项目名称）                |

### 1. 4 参考文献

​	[1] 邹欣.构建之法[M].第三版.人民邮电出版社,2017

## 二、项目概述

### 2. 1 产品描述

​		这是一款基于web网页的聊天听歌平台，用来与朋友、陌生人听歌聊天。借由本平台可以朋友之间，陌生人之间来感受音乐的魅力，体会音乐之美。

### 2. 2 产品功能

​	对于市面上的听歌软件都是单人听歌，少有做到多人同时在线听歌聊天。由此作为启发，我们提出了基于web网页的聊天听歌平台，可以与平台在线的网友同听一首歌并进行实时聊天。

### 2. 3 一般约束

​	进行本项目开发工作的约束条件如下：

#### 		2. 3. 1 开发环境约束

​		开发工具：IDEA

​		 测试工具：Chrome

​		开发语言：Java、JavaScript、HTML

#### 		2. 3. 2 时间约束

​		开发周期短，一个月的开发时间需要开发者合理规划时间，对于刚成立的团队和生疏的操作还需要磨合。

#### 		2. 3. 3 技术约束

​		所采用的方法与技术有限，项目团队成员的技术水平不够成熟，需要在开发中并发学习多种技术和能力。

### 2. 4 假设与依据

​	本项目是否能够成功实施，主要取决于以下的条件：

1. 团队成员的积极合作配合，为了项目的开发和实施，对个人时间进行合理规划同时为团队做出合理牺牲，配合队友完成任务。

2. 开发过程中遇到的技术问题可以及时得到同学或者老师的指导和帮助。

3. 团队掌握先进的能够适用于该项目的技术，这是系统的性能是否优化和项目能否成功的保证。

## 三、用户场景

### 场景1

典型用户：小洁（学生）

用户需求：听自己喜欢歌手的歌

场景描述：小洁同学是一名大三的学生，最喜欢的明星就是李易峰，每次他出了什么新的歌曲或者新专辑，都是第一时间去听，还喜欢和和大家分享自己喜欢歌手的歌曲。她发现了OMCP这个既可以听歌又可以聊天的网站就果断选择了，因为这不仅可以听自己喜欢听的歌曲还可以和别人一起分享表达自己对歌曲理解与看法。

### 场景2

典型用户：小刘（上班族）

用户需求：放松，舒缓压力

场景描述：小刘是一个程序员，典型地上班族每天过着朝九晚五的生活，平时加班的时间也比较多，工作压力较大，他比较希望自己能在下班时间或者空闲的时间能听歌和他人聊天放松一下自己，舒缓一下自己心情。当他用了OMCP这个听歌的网站后，自己确实放松了不少，因为公共聊天室里面有很有趣的话题。

### 场景3

典型用户：老黄（退休工人）

用户需求：消磨时间

场景描述：老黄是一名退休工人，平时的空闲时间较多，自己平时也喜欢唱歌，听歌，当他偶然发现OMCP这个听歌网站后，非常的满意，每天都要进去听听。

## 四、具体需求
### 4. 1 用例图
![8](https://img-blog.csdnimg.cn/20200609124042833.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
### 4. 2 类图
![9](https://img-blog.csdnimg.cn/20200609130628465.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
### 4. 3 顺序图
- TextArea：边界类
- ChatSystem：控制类
- ChatArea：边界类
![1](https://img-blog.csdnimg.cn/2020060912194891.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
- Form：边界类
- BackgroundSystem：控制类
- DataBase：辅助类
- Logininteface：边界类
![2](https://img-blog.csdnimg.cn/20200609122717656.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
- Form：边界类
- BackgroundSystem：控制类
- DataBase：辅助类
- MainPage：边界类
![3](https://img-blog.csdnimg.cn/20200609123000489.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
- SearchBar：边界类
- SerchSystem：控制类
- API：辅助类
- Resultlist：实体类
- SelectSong：控制类
- SongsManageSystem：控制类
- SongsList：边界类
![4](https://img-blog.csdnimg.cn/2020060912322967.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
- VoteWindow：边界类
- PromptSystem：控制类
- SongList：辅助类
![5](https://img-blog.csdnimg.cn/20200609123328871.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
- PromptSystem：控制类
- SongList：实体类
![6](https://img-blog.csdnimg.cn/20200609123424616.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)
- Songlist：边界类
![7](https://img-blog.csdnimg.cn/20200609123517836.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dlaXhpbl80NTczMzA0Nw==,size_16,color_FFFFFF,t_70)

### 4.4 外部接口需求

#### 	4.4.1 用户接口

​		无特殊需求。

#### 	4.4.2 硬件接口

​		无特殊需求。

#### 	4.4.3 软件接口

​		网易云API。

#### 	4.4.4 通信接口

​		无特殊需求。

## 五、界面原型

### 5. 1 主页

### 5. 2 注册登录页面

### 5. 3 我的

### 5. 4 歌单管理

## 六、功能描述

## 七、验收验证标准

### 7. 1 文档验收标准

- 文档编写符合国际文档编写规范
- 项目选题报告
- 软件按需求规格说明书

### 7. 2 软件验收标准

​	软件功能正常，bug不容易触发，运行流畅、不卡顿、适配于大部分能运行Chrome的电脑。

### 7. 3 界面验收标准

| 序号 | 界面名称     | 界面描述                                                     |
| ---- | ------------ | ------------------------------------------------------------ |
| 1    | 注册         |                                                              |
| 2    | 登录         |                                                              |
| 3    | 我的         | 左上角：返回<br />垂直线（由上到下）：修改头像、修改ID、我的收藏、歌单管理、退出登录 |
| 4    | 主页         | 标题栏：logo、歌曲搜索、账户中心<br />左区域：歌曲图片、进度条、音量条、投票切歌<br />右区域：聊天区 |
| 5    | 歌单管理页面 | 左上角：返回<br />                                           |

### 7. 4 功能验收标准

​	我们希望的小程序实现以下几点：

- 对于游客身份，做好游客的权限限制，仅能拥有的操作只是听歌和查看主页内容
- 游客注册时，需记录用户名和密码，并调用后台数据库验证是否合法，合法性判断将验证用户名是否已被使用
- 用户进入主页后，能拥有的操作有：听歌、聊天、点歌、投票切歌
- 管理员登录后可以进入歌单管理页面对歌曲进行管理
- 当用户点击投票切歌时，所有在线用户都会收到投票切歌提醒，当投票人数超过在线用户人数半数时，直接切换到下一首

### 7. 5 亮点以及未来预期完成的功能

​	我们预想了一下项目基本功能完成后的附加项，希望能够加以实现：

- 当歌单为空且超过五分钟无用户点歌时，将自动从API随机获取歌单并加入到OMCP歌单中
- 聊天可以发送系统提供的表情
- 我的收藏中的歌曲可以提供歌曲链接进行跳转

## 八、工作分配

| 人员 | 何昆佰 | 刘超然 | 高洁 | 黄波 | 刘丙亮 | 林金 | 李安娜 | 蒋晨 |
| :--: | :----: | :----: | :--: | :--: | :----: | :--: | :----: | :--: |
| 比例 |        |        |      |      |        |      |        |      |

