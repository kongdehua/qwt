# animation

使用的qwt类型：
* QwtPlot
  A 2D plotting widget
	
	QwtPlot is a widget for plotting two-dimensional graphs.
	An unlimited number of plot items can be displayd on its canvas. Plot items may be curves (QwtPlotCurve), markers (QwtPlotMarker), the grid (QwtPlotGrid), or anything else derived from QwtPlotItem.
	A plot can have up to four axes, with each plot item attached to a x- and a y axis, The scales at the axes can be explicitly set (QwtScaleDiv), or are calculated from the plot items, using algorithms (QwtScaleEngine) which can be configured separately for each axis.

	The simpleplot example is a good starting point to see how to set up a plot widget.

* QwtMath
* QwtSymbol
* QwtCurveFitter
* QwtPlotCurve
* QwtPlotCanvas
* QwtPlotLayout

示例中首先定义了QwtPlot的子类Plot：
类中首先禁用了所有数轴，设置空白区域

定义多条曲线，关键是将多条曲线附加到plot中
附加曲线：就是将数据线

更新曲线，所谓更新曲线，实质上就是更新数据。

更新数据：使用updateSamples就可以了。

