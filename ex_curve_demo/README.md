# Curv demo
用到以下qwt类型：
* qwt_scale_map

	QwtScaleMap offers transformations from the coordinate system of a scale into the linear coordinate system of a paint device and vice versa.

* qwt_plot_curve
* qwt_symbol
* qwt_math

qt类型就不管了

## 简要描述
This example program features some of the different display styles of the QwtPlotCurve class.

## 程序描述
首先定义MainWin，继承自QFrame
构造函数中设置QwtScaleMap的间距

设置边框属性

计算曲线值

定义多条曲线的风格，设置符号，设置画笔，设置风格，设置填充属性

绘制流程如下：
* 通过contentsRect()函数得到空间的坐标区域，QPainter用来绘制

* 主要使用QPainter设置属性，然后调用各自的draw函数，通过xMap和yMap来控制绘制区域，QwtScaleMap主要用来控制两个坐标系的转换

* 使用painter的drawText函数实现绘制字符串




