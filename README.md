Unofficial-API_for_Crawling
===========================
# 声明：
该源码仅为学习交流使用，不用于商业用途，如有侵权问题

请在[Issues](https://github.com/ClericPy/EC-Spider/issues)里留言

## 介绍：

文件名：get_jd.py

用途：非官方-京东商品爬虫API（包括价格、评论等），评分在评价的返回页面里有，销量暂时无法抓取。

抓取所有评论页耗费时间：

Python2 :3.19 s

Python3 :4.21 s

## 函数说明：
get_jd_rate：根据商品ID与页码获得评论页面的源代码，后续解析工作暂时不做了，就是解析Json

get_jd_rate_totalpagenum：根据商品ID得到评论页码范围，返回值是整型数字，最大页码-1，因为从0开始

get_jd_rate_all：根据商品ID抓取所有评论，返回结果是按顺序存放页面源码的列表

get_jd_price：根据商品ID抓取价格，这个速度最快，而且从来不会封IP

###### modifie：2014-11-09 11:23:36
