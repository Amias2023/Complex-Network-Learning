# 文献阅读



## 1. [《人类行为时空特性的统计力学》](https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Papers/%E4%BA%BA%E7%B1%BB%E8%A1%8C%E4%B8%BA%E6%97%B6%E7%A9%BA%E7%89%B9%E6%80%A7%E7%9A%84%E7%BB%9F%E8%AE%A1%E5%8A%9B%E5%AD%A6-%E5%91%A8%E6%B6%9B.pdf)-------周涛 电子科技大学报 2013年
> 关于人类行为  研究进展方向 详细介绍， 也有未来研究方向的见解 

### 一. 人类行为的时间特性

* 泊松分布 

    > 随机模型假设：在不重叠的时间区间 发生的次数相互独立

* 幂律分布  

    > 胖尾特征： 尾部下降时间缓慢，允许非常长的时间没有事情发生

* 阵发性

    > 很多事情在很短的时间内发生，出现较长的空档期------刻画标准： （平均值和标准值）


* 记忆性

    > 长的时间间隔之后出现长的时间间隔，短的时间间隔之后出现短的时间间隔------衡量标准：  序列的Pearson关联


* 周期和波动

    > 活跃性（单位时间个体特定行为的频数） 随着时间波动，而且具有明显的周期性



### 二. 人类行为的时间特性建模

####  1. 经典的基于任务队列模型

> 分配 l 个任务的列表，每一个时步个体选择执行一个任务，并且去除任务， 之后加入新的任务，并且标定他的优先级

> * 先进先出 -执行任务

> * 随机执行任务

> * 按照任务的优先级 执行任务

* Barabasi 模型
  
   >  对于每一个时步： 执行最高优先级的概率是P； 随机选取一个的概率是  1-P
  
* Barabasi模型拓展

   >  添加接受任务速度和完成任务速度


**总的人类行为的两大普适类**

* 长度固定，幂指数 = -1 

* 动态可变的，幂指数 - 1.5


####  2. 人类活动的记忆兴趣和节律

* 记忆模型

    > 记忆： 简单的表达为某件事情前后频率和次数的相关性

* 兴趣和欲望的自适应变化

    > 1）每次行为都会改变行为的兴趣，2） 时间间隔小，事件的额频率较高，兴趣减小，时间间隔增加。


#### 3.  基于社会交互的人类动力学模型
 * 扩展的任务队列模型


### 三. 人类行为空间特性分析

#### 1. 偏好返回模型

> * 1）初始 t= 0 ， 个体在给定的若干初始点的某一点进行停留

> * 2) 停留delta_t 时间后（服从一定的分布）， 个体以 P 的概率移动到之前没访问过的点， 以1-P的概率 移动到之前已经访问过的点（具体访问哪个点的概率==频率）

#### 2. 层次性交通系统对人类出行行为影响的模型

> * 城市分成n个层次， 两个第n层的城市同一个较高级的城市相连，他们之间相互🔗

> * 个体在网络中进行随机行走

> * 根据实际情况，引入城市权重，选择下一个城市的几率正比于 权重（使情况而定 之间的相互关系）


#### 3. 信息熵优化模型

* 返家机制的莱薇飞行模型

* 信息多样化程度


### 4. 研究方向

* 人类空间的运动规律研究
  >  现有研究： 移动步长分布，扩散速度等
  >  未来方向； 人类空间运动轨迹的规则性，周期性，相似性等等 + 考虑人类活动的社会性因素
  >  应用前景： 合理规划交通

* 人出行 和 网络中表现出的阵发性和记忆性
  > 用于异常行为检测

* 基于层次性交通网络人类的运动 👍 

* 空间位置预测

  > 考虑时间的动态贝叶斯预测
  > 转换为分类问题，使用神经网络和决策树
  
  

------------------
-----------------

## 2.  [利用移动网络数据的人类时空行为分析及建模研究](https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Papers/%E5%88%A9%E7%94%A8%E7%A7%BB%E5%8A%A8%E7%BD%91%E7%BB%9C%E6%95%B0%E6%8D%AE%E7%9A%84%E4%BA%BA%E7%B1%BB%E6%97%B6%E7%A9%BA%E8%A1%8C%E4%B8%BA%E5%88%86%E6%9E%90%E5%8F%8A%E5%BB%BA%E6%A8%A1%E7%A0%94%E7%A9%B6--%E5%8D%9A%E5%A3%AB%E8%AE%BA%E6%96%87.pdf)------ 博士论文  陈夏明博士  2016年
> 简介了人类个体行为的微观，宏观研究； 提出了 人类行为的介观表述； 人类个体行为抽象为有向属性图； 研究人类群体行为； 

<div align="center"> <img src="https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Image/%E4%BB%8B%E8%A7%82%E8%A1%A8%E8%BF%B0%E4%BA%BA%E7%B1%BB%E4%B8%AA%E4%BD%93%E8%A1%8C%E4%B8%BA.png" width="400"/> </div><br>



* 时空行为的研究角度

  > 物理学： 基于统计力学，将个体看作粒子，群体看作受限的粒子系统

  > 计算机： 数据挖掘和 机器学习


* 行为模式挖掘
  > 从历史轨迹数据中，发现移动的模式
  
  >>> 1) 无时间序列模式： 机器学习算法，进行相似轨迹的聚类分析。  👍
  
  >>> 2) 时空序列模式： 保留马尔可夫过程 ；加入： 停留时间，移动间隔时间，到达时间等（对应不同的）
  
 * 个体序列模式研究
 
  > 微观相似性： 采用序列的数据挖掘，从多个轨迹序列中提取出满足一定出现频次的子序列 👍
  
 * 群体模式研究
  
  > 人类动力学： 宏观统计，不同地点间的人数迁移规律： 辐射理论
  
  
  
  **研究方向**
  
  * 个体行为模式发生变化的成因及演化分
  
  * 用户行为和场景信息的关联分析  👍
  
  
  -------------
  ------------
  
  ## 3. [Trajectory Data Mining- An Overview](https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Papers/Trajectory%20Data%20Mining-%20An%20Overview.pdf)   ------郑宇博士，微软亚洲研究院 ，ACM Transactions on Intelligent Systems and Technology ，2015年
  
  <div align="center"> <img src="https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Image/trajectory_datamining.png" width="400"/> </div><br>
  
  
  * 自制的阅读记录

<div align="center"> <img src="https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Image/trajectory%20Data%20Mining.png" width="1600"/> </div><br>
  


------------
------------

## 4. [Introduction to TrajectoryDatamining--course](https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Papers/introduction%20to%20TrajectoryDatamining--course.pdf)  ----Kirsi Virrantaus Aalto University GIS-E4020

* Semantic Trajectories Modeling and Analysis

* Space-time density of real data

* 数据集： 轮船运行轨迹数据集，， 龙卷风数据集

-----------
---------

## 5. [Trajectory data mining- A review of methods and applications](https://github.com/LiuChuang0059/ComplexNetwork-DataMining/blob/master/Papers/Trajectory%20data%20mining-%20A%20review%20of%20methods%20and%20applications--2016.pdf)------Jean Damascène Mazimpaka and Sabine Timpf Department of Geography, University of Augsburg, Germany----  JOURNAL OF SPATIAL INFORMATION SCIENCE----2016







































