---
title: HTML简单时间控件
tags: html
categories: 前端
---
>#### Input Date 对象
Input Date 对象是 HTML5 中的新对象。
>Input Date 对象表示 HTML < input type="datetime"> 元素.注释：Internet Explorer 或 Firefox 不支持 < input type="date"> 元素。
## 1.日期时间( < input type=”datetime-local”/>)
既显示日期组件，又显示时间组件。

chrome效果
![datetime](/images/datetime.png)
手机效果
![phone](/images/phone.png)
## 2.日期(< input type=”date”/>)
显示日期

chrome效果 ![date](/images/date.png)
edge效果 ![date2](/images/date2.png)
## 3.时间(< input type=”time”/>)
这是最简单的一种显示，没有日历，只能选择时间。

chrome效果![time](/images/time.png)
edge效果![time2](/images/time2.png)
## 4.月份(< input type=”month”/>)
显示月份，跟“date”类型比起来少了后面的日子。

chrome效果![month](/images/month.png)

## 5.周(< input type=”week”/>)
显示周。注意周数显示的方式。

chrome效果![week](/images/week.png)

#### 除了以上类型为，日期输入类型还有一些其它属性。
| 属性        | 描述    |
| --------   | -----:   |
| value        | 这是HTML里input元素的通用属性。就是输入框里的数据      |   
| min        | 日期或时间的最小值      |   
| max	        | 日期或时间的最大值|
