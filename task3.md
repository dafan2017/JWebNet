## 智能高校在线答疑系统需求分析

### 1.引言
#### 1.1编写目的
本文档，为智能高校在线答疑系统提供需求分析文档，主要用于编程人员进行查阅。
#### 1.2背景
随着高校内学生人数的增长，教师和上课地点的不断变动使得    学生和老师之间的交流受时间和空间限制，导致师生间的答疑工作难以开展。为此开发一个智能高校在线答疑系统，来解决这种困境。由西安电子科技大学JW笃行团队提出并实施。
系统最终用户：高校学生、老师及管理人员
#### 1.3参考资料

Java核心技术 作 者：[美]霍斯特曼，[美]康奈尔  著   
深入体验Java Web 项目开发 作者：张玲玲 著

### 2.任务概述
#### 2.1目标
为了高校解决师资与学生不对等的问题，解决师生之间答疑的效率和便携性，更好地提升教学质量
#### 2.2用户特点
本系统中，只有三类用户，学生，教师和管理员，都是不具备计算机专业基础的使用者。
#### 2.3假定和约束
根据用户特点的约束，所以最终的项目成品系统的可交互性要足够好，让人能够一眼就看到系统所有的功能，并且使用控件就可以完成所需要的要求。
### 3.需求规定
#### 3.1对功能的规定
该系统包括三类用户，分别为学生用户、教师用户和管理员用户，其各项功能如下：
##### （1）学生端
·注册用户和登陆：学生可自由地注册用户并登陆在线答疑系统  
·资料修改与密码修改：注册后的学生可以修改自己的资料和密码  
·查询问题：可查看所有问题，也可以采用模糊搜索搜索已存在的问题，和相应的回答  
·查看参与的提问：学生可以查看自己所有参与的问题并可以追加提问。  
·新建提问：学生通过可以新建一个问题，并选择回答对象。  
##### （2）教师端
·查看未回答的问题：登陆后，教师可以查看未回答问题列表
·查看已回答问题：对于已回答的问题可以继续追加回答。
·资料上传：可以上传相关的学习资料
·收藏问题：教师可以收藏一些好的提问，并可以下载。
·提问：老师也可以对同学们提出问题。
##### （3）管理端
·用户管理：管理教师用户和学生用户，可以重置用户的密码
·内容管理：管理员可以对提问内容和回复内容进行管理。
·管理员管理：超级用户对一般管理员的管理
·禁止操作：对不合法或者言语攻击等的用户进行禁言或者删除用户操作。
#### 3.2对性能的规定
##### 3.2.1数据库要求
数据库要求能承载系统的数据量，本系统属于小型系统，因此使用Sql Server 或者mysql等数据库就可以满足要求。
##### 3.2.2服务器
能在windows平台下运行的服务器，能支撑动态网站开发的服务器并且，必须是免费的，因此选择tomcat服务器
##### 3.2.3友好的用户界面
必须提供一个友好的用户界面，使用最便捷的操作，完成系统功能。并且应该给予最清晰的提示。
### 4.运行环境规定
Eclipse：一个十分优秀的用于开发Java, J2EE的Eclipse插件集合，MyEclipse的 功能非常强大，支持也十分广泛，尤其是对各种开源产品的支持十分不错。  

JDK：JDK 是整个Java的核心，包括了Java运行环境、Java工具和Java基础类库。  

数据库：MySql 数据库是目前小型应用开发中比较流行的数据库，并且支持事务机制，也有保证数据完整性和安全性的能力。 

控制层：Struts 2是Struts的下一代产品，是在 struts 1和WebWork的技术基础上进 行了合并的全新的Struts 2框架。其全新的Struts 2的体系结构与Struts 1的体系结构差别巨大。Struts 2以WebWork为核心，采用拦截器的机制来处理用户的请求，这样的设计也使得业务逻辑控制器能够与ServletAPI完全脱离开，所以Struts 2可以理解为WebWork的更新产品。虽然从Struts 1到Struts 2有着太大的变化，但是相对于WebWork，Struts 2的变化很小。  

业务层：Spring 3.0版本采用优秀的JavaEE 开源框架，其提供的控制反转及面向方面 的编程插件式架构降低了应用组件之间的依赖性。
