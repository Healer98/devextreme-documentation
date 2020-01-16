The *win-loss* series type will suit you best when you need to demonstrate whether or not some values have had success in exceeding a specific threshold value. This series type strongly resembles the [bar](/concepts/20%20Data%20Visualization/10%20Charts/38%20Sparkline%20Series%20Types/070%20Bar.md '/Documentation/Guide/Data_Visualization/Charts/Sparkline_Series_Types/#Bar') series type. The fundamental difference is that while in a *bar* series, bars are classified as being greater or less than zero, in a *win-loss* series, they are classified as being greater or less than a specific value called "threshold".

![DevExtreme ChartJS Sparkline](/images/ChartJS/SparklineWinLoss.png)

To specify the *win-loss* series type, assign *'winloss'* to the [type](/api-reference/20%20Data%20Visualization%20Widgets/60%20dxSparkline/1%20Configuration/type.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxSparkline/Configuration/#type') option of the main configuration object.

	<!--JavaScript-->var sparklineOptions = {
		type: 'winloss',
		// ...
	};

After that, specify the value to be used as the threshold. Assign this value to the [winlossThreshold](/api-reference/20%20Data%20Visualization%20Widgets/60%20dxSparkline/1%20Configuration/winlossThreshold.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxSparkline/Configuration/#winlossThreshold') option.

	<!--JavaScript-->var sparklineOptions = {
		winlossThreshold: 2000,
		// ...
	};

The color of a particular bar in a *win-loss* series depends on the value it represents. If this value is greater than the threshold, this bar is painted in a "win" color. Otherwise, it is painted in a "loss" color. These colors can be specified using the [winColor](/api-reference/20%20Data%20Visualization%20Widgets/60%20dxSparkline/1%20Configuration/winColor.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxSparkline/Configuration/#winColor') and [lossColor](/api-reference/20%20Data%20Visualization%20Widgets/60%20dxSparkline/1%20Configuration/lossColor.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxSparkline/Configuration/#lossColor') options.

In addition, you can indicate extreme points on a *win-loss* sparkline. To learn how to do this, refer to the [Series Points](/concepts/20%20Data%20Visualization/10%20Charts/37%20Sparkline%20Elements/20%20Series%20Points.md '/Documentation/Guide/Data_Visualization/Charts/Sparkline_Elements/#Series_Points') topic.

<a href="http://js.devexpress.com/Demos/WidgetsGallery/#demo/chartssparklinessparklineswinloss/" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>