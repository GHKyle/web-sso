ki4so
=====

#产品发布计划
##ki4so 2015新年贺岁版本发布计划
产品发布时间： 2015. 1.1 （新年贺岁版） 
产品包括的特性： 
1.统一登入 （提升质量，详细测试）
2.统一登出（后端实现稳定可靠的统一登出）。 
3.java通用客户端。 
4.产品使用和开发文档。 降低使用难度，
5.java客户端应用demo。演示如何集成ki4so
6.可供直接下载的war包。
7.项目迁移到oschina上维护。提升访问速度和稳定性。



#下载地址
等待打包和发布最新版本


#项目介绍
##简介
ki4so是一个简约、无状态、易扩展、易伸缩的适合于大型互联网web应用场景的单点登录系统，它功能简单，只实现了统一登录和登出，它最大的特色是将用户状态写入到cookie中，最大程度减少了单点登录服务端的状态，服务端只需要存储公共的应用密钥，将用户凭证的认证分散到各应用服务中，最大程度减轻了ki4so服务器的压力。
##名称由来
ki4so，英文全称是：kiss sso意思是简约单点登录系统，由于s太多，名字看起来比较繁琐，我们缩写为4s，跟汽车的4s店一样，我们会为使用ki4so的用户提供全方位、细心周到的4s服务，我们会用自己最真诚的心态来对待该项目，努力打造一个对用户有价值，用户体验很好，技术支持及服务用心的技术产品。
##项目由来
我们所在的公司内部一直在使用耶鲁大学的[CAS](https://github.com/ywbrj042/cas "CAS")作为自己的单点登录系统，在功能上能够满足自己的需求，但是觉得它太重量级，有状态，不太适合于互联网应用，因此2013年5月我们打算开发一个更加轻量级、简单、适合互联网应用的开源sso系统，因此本项目诞生了。

#为什么要用ki4so？
单点登录系统有很多，开源的成熟的产品也有很多，比如耶鲁大学的cas等。

1. 无状态。系统可伸缩性好。
2. 简单轻量级。
3. 性能高。
4. 安全性高。
5. 质量高，有大量的单元测试保障代码质量。

#ki4so常见问题指南

[ki4so常见问题指南](https://github.com/ebnew/ki4so/blob/master/docs/user/FAQ.md "ki4so常见问题指南")

#ki4so安装使用说明

[ki4so服务器快速安装说明](https://github.com/ebnew/ki4so/blob/master/docs/user/INSTALL.md "ki4so服务器快速安装说明")

[ki4so服务器配置详细说明](https://github.com/ebnew/ki4so/blob/master/docs/user/KI4SO_SERVER_CONFIG.md "ki4so服务器配置详细说明")

[ki4so客户端配置详细说明](https://github.com/ebnew/ki4so/blob/master/docs/user/KI4SO_CLIENT_CONFIG.md "ki4so客户端配置详细说明")

[ki4so客户端开发包协议说明](https://github.com/ebnew/ki4so/blob/master/docs/user/KI4SO_CLIENT_DEV_GUIDE.md "ki4so客户端开发包协议说明")


#ki4so代码质量
##ki4so-core工程代码测试覆盖率

![ki4so-core工程代码测试覆盖率](http://github.com/ebnew/ki4so/raw/master/images/cobertura_ki4so_core.jpg)

##ki4so-web工程代码测试覆盖率

![ki4so-web工程代码测试覆盖率](http://github.com/ebnew/ki4so/raw/master/images/cobertura_ki4so_web.jpg)

##ki4so-common工程代码测试覆盖率

![ki4so-common工程代码测试覆盖率](http://github.com/ebnew/ki4so/raw/master/images/cobertura_ki4so_common.jpg)





#交流方式

我们的QQ群号是：199315835。本项目的核心成员都在里面，请加入该群提问。

#项目许可协议
项目遵循[Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)开源协议

#产品状态
目前ki4so处于1.0.1-SNAPSHOT的开发期，目前还没有可以发布正式可以用的版本。目前产品完成的需求如下：
a.完成统一登录。

b.完成统一登出。目前统一登出是在客户端实现，使用jsonp实现，原生的javascript，不依赖任何lib包。集成非常简单。

c.客户端目前只完成了java原生应用客户端，其它语言暂时未开发。

d.单元测试正在持续补充中，引入了代码覆盖率检查工具，依据覆盖率进行代码测试。性能优化是下一步要做的事情。

e.代码结构有待优化。


#项目版本号说明

当前版本号：1.0.0-SNAPSHOT

本项目采用通用的三级版本号，版本号格式是[主版本号].[副版本号].[修复版本号]-[稳定状态]，如：1.0.0-SNAPSHOT。

1. [主版本号] 是从1开始的整数，表示重大的项目结构和概念调整，一般不会轻易修改该版本号，不同的主版本号不承诺能够兼容。
2. [副版本号]是从0开始的整数，表示项目的功能特性增加或者BUG修复，同一个[主版本号]下的不同副版本是能够向下兼容的。
3. [修复版本号]的只是从0开始的整数，一般只是小的BUG修复，细微功能调整。
4. [稳定状态]的可选值有：SNAPSHOT、RC[序号]、RELEASE。SNAPSHOT表示开发快照版本，该版本未经过严格测试，可能呢不稳定，不宜用于生产环境；RC[序号]表示可选非正式发布版本，比较稳定，但是非正式版本，可能存在问题，可能有多个RC版本，RC序号会有多个；RELEASE表示正式发布版本，经过了严格测试，可以用于生产环境，请尽量用该版本作为生产使用。



#项目目录说明
在项目代码的根目录下分别有如下文件目录，含义分别如下：

1. docs 该目录下存放的是各种项目文档，包括架构设计、概要设计、详细设计、用户手册、和安装手册等，我们承诺本项目将成为文档最全的项目之一，方便所有人学习和使用。 子目录的说明请查看目录下的README.md文件。
2. pom.xml。该文件是maven工程描述文件，其它的两个目录ki4so-core和ki4so-web都是两个maven工程，具体请参考描述文件说明，若不了解maven是什么，请google之。


#谁在用ki4so?

暂无，持续收集中。

