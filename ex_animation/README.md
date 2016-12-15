# animation

ʹ�õ�qwt���ͣ�
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
	A plot item, that represents a series of points

	A curve is the representation of a series of points in the x-y plane. It supports different display styles, interplation and symbols.


* QwtPlotCanvas
* QwtPlotLayout <--- QwtWidgetOverlay
	An overlay for a widget

	The main use case of an widget overlay is to avoid heavy repaint operation of the widget below.

	F.e. in combination with the plot canvas an overlay avoid replots as the content of the canvas can be restored from its backing store.

	QwtWidgetOverlay is an abstract base class. Deriving classes are supposed to reimplement the following methods:
	- drawOverlay()
	- maskHint()

	Internally, QwtPlotPicker uses overlays for displaying the rubber band and the tracker text.

ʾ�������ȶ�����QwtPlot������Plot��
�������Ƚ������������ᣬ���ÿհ�����

����������ߣ��ؼ��ǽ��������߸��ӵ�plot��
�������ߣ����ǽ�������

�������ߣ���ν�������ߣ�ʵ���Ͼ��Ǹ������ݡ�

�������ݣ�ʹ��updateSamples�Ϳ����ˡ�

## ����ʵ�ַ���
���ȶ���Curve���࣬�м�����һ��QTransform�������ƶ�����

Curve1�����У�����QwtSplineCurveFitter���߹�������������Ʒ��ţ�����Transformation��


