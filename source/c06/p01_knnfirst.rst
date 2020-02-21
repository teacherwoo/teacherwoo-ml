===============================
 K-近邻算法简介 
===============================


学习目标
--------------



什么是K-近邻算法
-----------------


根据你的“邻居”来推断出你的类别
1.1 K-近邻算法(KNN)概念
K Nearest Neighbor算法又叫KNN算法，这个算法是机器学习里面一个比较经典的算法， 总体来说KNN算法是相对比较容易理解的算法

定义
如果一个样本在特征空间中的k个最相似(即特征空间中最邻近)的样本中的大多数属于某一个类别，则该样本也属于这个类别。

来源：KNN算法最早是由Cover和Hart提出的一种分类算法

距离公式
两个样本的距离可以通过如下公式计算，又叫欧式距离 ，关于距离公式会在后面进行讨论

.. math::

   \begin{array}{*{20}{l}}
   {\text{已}\text{知}\text{点}A{ \left( {\mathop{{x}}\nolimits_{{1}},\mathop{{y}}\nolimits_{{1}}} \right) },\text{点}B{ \left( {\mathop{{x}}\nolimits_{{2}},\mathop{{y}}\nolimits_{{2}}} \right) }}\\
   {\text{则}\text{两}\text{点}\text{距}\text{离}}\\
   {d=\sqrt{{\mathop{{ \left( {\mathop{{x}}\nolimits_{{2}}-\mathop{{x}}\nolimits_{{1}}} \right) }}\nolimits^{{2}}+\mathop{{ \left( {\mathop{{y}}\nolimits_{{2}}-\mathop{{y}}\nolimits_{{1}}} \right) }}\nolimits^{{2}}}}}
   \end{array}



1.2 电影类型分析
假设我们现在有几部电影

image-20190316204421392

其中？ 号电影不知道类别，如何去预测？我们可以利用K近邻算法的思想

image-20190316204448303

分别计算每个电影和被预测电影的距离，然后求解

image-20190316204517137