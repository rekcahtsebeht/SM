# UML简单介绍(十八)——组件图的基本概念与实例解析
**1、组件图**

组件图又被成为构件图，主要用于静态建模，是表示构件类型的组织以及各种构件之间依赖关系的图。组件图通过对组件间依赖关系的描述来估
件的修改给系统可能带来的影响。

**2、事务**

可替换的物理部分包括软件代码、脚本或命令行文件，也可以表示运行时的对象，文档，数据库等。节点( node )是运行时的物理对象，代表一
源。事务的图示如下：

![image](https://github.com/rekcahtsebeht/SM/blob/main/1.drawio.png)

**3、关系**

组件图中的关系也 比较简单，主要是依赖和实现等，如下：

![image](https://github.com/rekcahtsebeht/SM/blob/main/2.drawio.png)

**4、实例**

图中的构件名称是Dictionary字典。该构件向外提供两个接口，即两个服务Spell-check拼写检查、Synonyms同义词。

![image](https://github.com/rekcahtsebeht/SM/blob/main/3.drawio.png)

图中“Planner计划者”构件向外提供一个“update更新”接口服务。同时，该构件要求外部接口提供一个“Reservations预定”服务。

![image](https://github.com/rekcahtsebeht/SM/blob/main/4.drawio.png)

**5、购票流程**

**5.1 情景描述**

情景一：

购买个人票可以通过公用信息亭订购也可直接向售票员购买，但购买团体票只能通过售票员。

情景二：

买票的人可以根据任意选择预订销售或个人销售或团体销售中的一种方式，售票处为了方便销售，需要信用卡付款服务的支持，同时也必然需要票数据
票可卖的状况中。

图示如下：

![image](https://github.com/rekcahtsebeht/SM/blob/main/5.drawio.png)

**5,2 图示关系**

图中依赖关系包括：顾客需要信息亭接口提供服务

售票员需要职员接口提供服务

信用卡付款需要信用卡代理提供服务

职员接口需要预订销售、个人销售和团体销售提供服务

管理接口需要数据库状态提供服务

售票处需要付款和购买提供服务

圖中實現包括:

信用卡付款提供付款服务

票数据库提供购买和状态查询服务

售票处提供预订购买、个人购买和团体购买服务


