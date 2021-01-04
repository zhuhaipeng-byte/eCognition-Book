# 编著：eCognition遥感图像处理实战

--------------------------------------------------------

# 前言
--------------------------------------------------------
## 为什么要写这本书
-------------------------------------------------------
&emsp; 随着航空航天技术的快速发展，高空间分辨率和时间分辨率的遥感卫星数据空前增加。在大数据时代，从海量的遥感卫星数据中挖掘信息、知识表示与
推理总结规律，是目前遇到的一个挑战。针对这些问题，eCognition具有先天优势。eCognition是以对象的遥感图像解译为指导的遥感应用分析平台，集成
了SVM、深度学习和超像素分割算法等机器学习算法。从并行处理能力来看，eCognition从单机版交互式影像分析进化到基于规则集开发模式的专业化影像分析，
进而升级为自动化海量影像并行处理系统。

&emsp; 但eCognition软件给行业带来福音的同时，也给读者提高了学习成本。eCognition软件概念体系复杂、算法特征参数类型繁多，而可参考的资料却
较少。eCognition软件引进国内十几年以来，用户与潜在用户不断增加。但截至目前还没有出版一本系统的操作性强的参考教材，大多数读者只是参加短期的
软件学习培训班，依靠软件自带的参考资料自己琢磨，费时费力，往往效果不佳，学习新技术的热情在不得法的学习过程中消磨殆尽。本书作者从2014年在推广
软件和实战中积累经验，不断提高软件应用能力，把工作中积累的经验全部分享出来，久而久之成为今天读者看到的这本书。

&emsp; 本书由致力于eCognition研发一线的高级工程师、高校教师与行业专家共同完成，兼顾高校教材特点和企业生产实际，将行业解决方案和生产实际应
用情况进行了系统结合。与编者参与的姊妹书《eCognition基于对象影像分析教程》相比，本书具有简化理论，注重操作实践的特色，以企业级的高标准来撰
写此书，主要面向高校教师、高年级本科生、研究生和生产一线的工程师，可作为他们学习与科研工作的参考资料。
## 主要内容
------------------------------------------------------------------
&emsp; 全书内容分为基础操作、行业解决方案和生产应用3篇，共9章。基础操作篇：第1章，主要介绍了eCognition 9.x软件概况、基础架构、产品组成和
特色，并对如何使用本书进行了介绍。第2章，对eCognition 9.x新增的模板匹配进行了分析，并对模板和非模板实际操作进行了介绍。第3章，以行业点云数
据分析为例，通过点云数据处理、点云信息和影像结合进行实际操作，让读者深入了解如何使用多源数据进行点云分析；解决方案篇：第4-6章，主要以解决方
案为导向，将转移图层分析、矢量数据分析、区域与地图分析等使用技巧与具体行业进行结合，带领读者将软件操作与行业进行深度融合，形成自己的解决方案；
生产应用篇：第7~9章，主要介绍eCognition9.x的eCognition Architect在生产中的使用技巧，让非专业人员也能娴熟的使用eCognition9.x。

&emsp; 本书参阅了国内外大量论著和学术论文，但仍难免挂一漏万，希望读者在使用过程中能够提出宝贵意见，以便我们持续改进。本书的部分案例及数据由美国
Trimble公司提供，在此表示感谢。本书的编写分工是：全教程的统稿和定稿由主编郝容（二十一世纪空间技术应用股份有限公司）、王学恭（天水师范学院资源与
环境工程学院）和郭涛（四川省农业科学院遥感应用研究所）完成；内容简介、前言和上篇等内容由郭涛、郝容和刘孟琴（西南科技大学环境与资源学院）编写；
中篇和下篇主要由浩容、马浩然、周菁和屈鸿钧编写，王学恭、郭涛进行了修改、调整和优化。此外，白洁和刘孟琴负责整本书的图片修饰、数据整理、实验验证和
校对工作。感谢中国气象科学研究院房世波研究员和自然资源部第三航测遥感院张平工程师长期的指导与帮助，并在百忙之中为本书作序。本书出版过程中，得到了
四川省农业科学院遥感应用研究所黄平、杨健和任国业等所领导的关心和大力支持，李源洪主任、刘轲博士、张敏、覃玥、董秀春等同事和朋友给予的鼓励与协助，
在此一并致以最真挚的感谢。此外，感谢本书的技术审核，他们是自然资源部四川基础地理信息中心周尧工程师，兰州大学王梅梅博士，中国地质大学（武汉）王雄，
吉林大学朱梦瑶，四川师范大学叶华丽、胡怡，西南科技大学郭家、李疆，感谢他们对本书做出的贡献。

## 勘误和支持
----------------------------------------------------------------------
&emsp; 本书以2019年12月10日最新发布的eCognition V9.5.1版本软件为主，试用版软件可以在：http://www.ecognition.com/free-trial 下载。
为了持续对本书进行更新，本书采用“Open Source Book”方式，采用OSB协议定期更新新增部分，新增部分以电子版方式开放。同时，希望各位读者对本书存
在的问题进行反馈，TIT Lab团队以3个月为固定周期进行新版本迭代更新，以便于本书能够持续更新。也鼓励读者将自己工作中涉及的技术形成文档，提交给我
们，我们将以开源、包容和尊重知识产权的态度，在后续新版书出版时一一进行注明。本书中案例的彩色图片、实验数据、eCognition技术文档和错误校勘可在
https://github.com/guotao0628/eCognition-Book 提交和下载。为了读者与本书作者能够深入开展交流，建立了两个QQ群：596706740、189303733，
欢迎同行加入参与讨论。

## 致谢
---------------------------------------------------------------------
&emsp; 本书编写思路2014年既由郝容提出，但受种种主客观因素的影响，这一好的想法并未得到及时落实。历时近5年的时间，直到2018年春，在大家的支持下
，才完成此书初稿。本书出版过程中得到了天水师范学院和四川省农业科学院遥感应用研究所的大力支持。科学出版社的杨红编辑为本书的出版付出了辛勤的劳
，做了大量细致的指导工作。美国Trimble公司eCognition中国业务负责人在协调案例的合法使用方面给予了极大的帮助，在此一并致以衷心的感谢！限于
编者的编撰水平，书中可能存在一些不当之处，敬请各位读者不吝赐教。


                                                                                                              
                                                                                                             王学恭                    
                                                                                          天水师范学院资源与环境工程学院
                                                                                          
                                                                                                               郝容
                                                                                 二十一世纪空间技术应用股份有限公司技术经理
                                                                                 
                                                                                                                郭涛
                                                                                            四川省农业科学院遥感应用研究所 
                                                                                            
----------------------------------------------------------------------------

更多关于出版的相关编著相关问题讨论，可提交到Github或者发Email：guotao3s@163.com.

-------------------------------------------------------------------------
       
