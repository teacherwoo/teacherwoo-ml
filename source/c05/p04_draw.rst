=====================
Pandas画图 
=====================

----------
学习目标
----------

 
了解DataFrame的画图函数
了解Series的画图函数
应用：股票每日数据的统计

pandas.DataFrame.plot
-----------------------------------

DataFrame.plot(x=None, y=None, kind='line')

x : label or position, default None
y : label, position or list of label, positions, default None
Allows plotting of one column versus another
kind : str
‘line’ : line plot (default)
‘bar’ : vertical bar plot
‘barh’ : horizontal bar plot
关于“barh”的解释：
http://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.plot.barh.html
‘hist’ : histogram
‘pie’ : pie plot
‘scatter’ : scatter plot
更多参数细节：https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.plot.html?highlight=plot#pandas.DataFrame.plot

pandas.Series.plot
---------------------------

更多参数细节：https://pandas.pydata.org/pandas-docs/stable/generated/pandas.Series.plot.html?highlight=plot#pandas.Series.plot