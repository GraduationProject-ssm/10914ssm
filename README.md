# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 10914ssm毕业生就业信息管理系统

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Sh44eDEx6?p=15)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

毕业生就业信息管理系统工作原理图如图4-1所示：

![](/md/blog.012.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。毕业生就业信息管理系统的整体结构设计如图4-2所示。

![](/md/blog.013.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
数据库的概念结构设计采用实体—联系（E-R）模型设计方法。E-R模型法的组成元素有：实体、属性、联系，E-R模型用E-R图表示，是提示学生工作环境中所涉及的事物，属性则是对实体特性的描述。在系统设计当中数据库起着决定性的因素。下面设计出这几个关键实体的实体—关系图。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，学校中的每个学生，家里中的每个学习用品。

本系统的E-R图如下图所示：

1、学生信息：学籍号、密码、学生姓名、学校、学院、专业、年龄、班级、联系电话、邮箱、身份证、就业导师、出生日期、学历，实体图如图4-3所示：

![](/md/blog.014.png)

图4-3学生信息实体图

2、就业导师信息：教师工号、密码、教师姓名、职称、电话、邮箱，实体图如图4-4所示：

![](/md/blog.015.png)

图4-4就业导师信息实体图

3、企业信息：企业账号、密码、企业名称、企业地址、企业规模、负责人、联系电话、邮箱,实体图如图4-5所示：

![](/md/blog.016.png)

图4-5企业信息实体图

#########

### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

allusers表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|username||150||255||
|3|pwd||150||255||
|4|cx||150||255||
|5|addtime|DateTime|8||19||

jiuyedaoshi表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|addtime||150||255||
|3|jiaoshigonghao||150||255||
|4|mima|DateTime|8||255||
|5|jiaoshixingming||150||255||
|6|xingbie|DateTime|8||255||
|7|zhicheng||150||255||
|8|dianhua|DateTime|8||255||
|9|youxiang||150||255||
|10|zhaopian|DateTime|8||255||

lijiebiyeshengjiuyexinxi表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|addtime||150||255||
|3|xueyuan||150||255||
|4|ruzhidanwei|DateTime|8||255||
|5|ruzhirenshu||150||255||
|6|xinchou|DateTime|8||255||
|7|qitadaiyu||150||255||

mianshiyaoqing表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|addtime||150||255||
|4|shifouluyong|DateTime|8||255||
|5|beiyaoqingrenxingming||150||255||
|6|xuejihao|DateTime|8||255||
|7|qiyezhanghao||150||255||
|8|mianshididian|DateTime|8||255||
|9|mianshishijian||150||255||

qiye表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|addtime||150||255||
|4|qiyezhanghao|DateTime|8||255||
|5|mima||150||255||
|6|qiyemingcheng|DateTime|8||255||
|7|qiyedizhi||150||255||
|8|qiyeguimo|DateTime|8||255||
|9|fuzeren||150||255||
|10|lianxifangshi|DateTime|8||255||
|11|qiyetupian||150||255||
|12|youxiang|DateTime|8||255||
|13|qiyejianjie||150||255||

toudidejianli表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|addtime||150||255||
|4|xuejihao|DateTime|8||255||
|5|xueshengxingming||150||255||
|6|zhuanye|DateTime|8||255||
|7|xingbie||150||255||
|8|mianshididian|DateTime|8||255||
|9|shenfenzheng||150||255||
|10|zhaopian|DateTime|8||255||
|11|chushengriqi||150||255||
|`	`12|gongsimingcheng|DateTime|8||255||
|13|qiuzhigangwei||150||255||
|14|gongzuodidian|DateTime|8||255||
|15|qiwangxinzi||150||255||
|16|jiaoyubeijing|DateTime|8||255||
|17|huojiangzhengshu||150||255||
|18|biyexuexiao|DateTime|8||255||
|19|xiangxineirong||150||255||

xuesheng表:

|序号|字段名称|字段类型|大小|允许为空|最大长度|备注|
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|1|id|Int|4||10||
|2|addtime||150||255||
|4|xuejihao|DateTime|8||255||
|5|mima||150||255||
|6|xueshengxingming|DateTime|8||255||
|7|xingbie||150||255||
|8|xuexiao|DateTime|8||255||
|9|xueyuan||150||255||
|10|zhuanye|DateTime|8||255||
|11|nianji||150||255||
|12|banji|DateTime|8||255||
|13|lianxidianhua||150||255||
||youxiang|DateTime|8||255||
||shenfenzheng||150||255||
||jiuyedaoshi|DateTime|8||255||
||zhaopian||150||255||
||chushengriqi|DateTime|8||255||
||xueli||150||255||
#
# 5统详细设计

## 5.1管理员功能模块
管理员输入个人的用户名、密码、角色登录系统，这时候系统的数据库就会在进行查找相关的信息，如果我们输入的用户名、密码不正确，数据库就会提示出错误的信息提示，同时会提示管理员重新输入自己的用户名、密码，直到账号密码输入成功后，会提登录成功的信息。网站管理员登录效果图如图5-1所示：

![](/md/blog.017.png)

图5-1管理员登录界面图

管理员登录进入毕业生就业信息管理系统可以查看首页、个人中心、学生管理、就业导师管理、企业管理、招聘信息管理、历届毕业生就业信息管理、面试邀请管理、投递的简历管理、系统管理等信息。如图5-2所示。

![](/md/blog.018.png)

图5-2首页界面图


历届毕业生就业信息管理，管理员在历届毕业生就业信息管理可以查看学院、入职单位、入职人数、薪资、其他待遇等信息，并可根据需要对已有就业信息进行详情、修改或删除等操作，如图5-3所示。

![](/md/blog.019.png)

图5-3历届毕业生就业信息管理界面图



## 5.2企业功能模块
企业注册、登陆，企业通过注册页面填写企业账号、密码、企业名称、企业地址、企业规模、负责人、联系电话、邮箱进行注册。信息无误进行填写企业账号、密码选择角色进行登陆，如图5-4所示。

![](/md/blog.020.png)

![](/md/blog.021.png)

图5-4注册、登陆界面图

首页，企业在首页页面中可以查看个人中心、学生管理、招聘信息管理、面试邀请管理、投递的简历管理等信息，如图5-5所示。

![](/md/blog.022.png)

图5-5企业首页界面图

招聘信息管理，企业在招聘信息通过页面查看招聘编号、企业名称、联系方式、邮箱、招聘人数、招聘岗位、照片、职位要求、工作待遇等信息，进行查询、添加、修改、删除操作，需要经过管理员或者就业导师审核才能进行应聘。如图5-6所示。

![](/md/blog.023.png)

图5-6招聘信息管理界面图

投递的简历管理，企业在投递的简历通过页面查看学籍号、学生姓名、学历专业、性别、身份证、照片、出生日期、公司名称、求职岗位、工作地点、期望薪资、教育背景、获奖证书、毕业学校、详细内容等信息，可进行面试邀请、查看详情。如图5-7所示。

![](/md/blog.024.png)

![](/md/blog.025.png)

图5-7投递的简历、面试邀请界面图


## 5.3学生前后功能模块
学生注册、登陆，学生通过注册页面填写学籍号、密码、学生姓名、学校、学院、专业、年龄、班级、联系电话、邮箱、身份证、就业导师、出生日期、学历进行注册。信息无误进行填写学籍号、密码选择角色进行登陆，如图5-8所示。

![](/md/blog.026.png)

![](/md/blog.027.png)

图5-8注册、登陆界面图

首页，学生登陆进入前台首页查看首页、招聘信息、新闻资讯、我的、跳转到后台等信息，如图5-9所示。

招聘信息，学生在前台首页点击招聘信息进行查看招聘编号、企业名称、联系方式、邮箱、招聘人数、招聘岗位，可进行投递简历操作，如图5-10所示。

![](/md/blog.028.png)

图5-10首页界面图

![](/md/blog.029.png)

![](/md/blog.030.png)

图5-11招聘信息界面图

首页，学生在首页页面中可以查看个人中心、企业管理、招聘信息管理、历届毕业生就业信息管理、面试邀请管理、投递的简历管理等信息，如图5-12所示。

![](/md/blog.031.png)

图5-12学生后台首页界面图

投递的简历管理，学生在投递简历页面查看学籍号、学生姓名、学历专业、性别、身份证、照片、出生日期、公司名称、求职岗位、工作地点、期望薪资、教育背景、获奖证书、毕业学校、详细内容等信息，进行查看操作，如图5-13所示。

![](/md/blog.032.png)

图5-13投递简历界面图

面试邀请管理，学生进入面试邀请查看，可进行学生姓名、学历、专业、求职岗位进行查询操作，如图5-14所示。

![](/md/blog.032.png)

图5-14面试邀请界面图

## 5.4就业导师功能模块
就业导师登陆，就业导师通登陆页面填写教师工号、密码选择角色进行登陆，如图5-15所示。

![](/md/blog.033.png)

图5-15登陆界面图

首页，就业导师在首页页面中可以查看个人中心、学生管理、企业管理、招聘信息管理、历届毕业生就业信息管理、系统管理等信息，如图5-16所示。

![](/md/blog.034.png)

图5-16就业导师后台首页界面图

招聘信息管理，就业导师在招聘信息通过页面查看招聘编号、企业名称、联系方式、邮箱、招聘人数、招聘岗位、照片、职位要求、工作待遇等信息，进行查询、审核、修改、删除操作，如图5-17所示。

![](/md/blog.035.png)

图5-17招聘信息管理界面图

历届毕业生就业信息管理，就业导师在就业信息通过页面查看学院、入职单位、入职人数、薪资、其他待遇等信息，进行查看操作，如图5-18所示。

![](/md/blog.036.png)

图5-19历届毕业生就业信息界面图












