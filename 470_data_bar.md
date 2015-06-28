# 3.7.0 Data Bar Formatting

Top/Bottom Percentile Formatting allows you to set up a formatting condition that will either highlight a top or bottom percentile of values in a given range, or it will highlight a number of top or bottom values. 

![](databar_1.png)

### 3.7.1 Define Formatting Condition Rules

<blockquote>

<p><b>MinType:</b> [Condition Value Type] If this input is LowestValue or AutomaticMin Excel will automatically assign the minimum value from the range of numbers specified. MinValue will NOT need to be supplied if either one of the two values are used.</p>

<p><b>MinValue:</b> [Integer]  Only needed if MinType IS NOT LowestValue or AutomaticMin </p>

<p><b>MaxType:</b> [[Condition Value Type] If this input is HeighestValue or AutomaticMax Excel will automatically assign the maximum value from the range of numbers specified. MaxValue will NOT need to be supplied if either one of the two values are used.</p>

<p><b>MaxValue:</b> [Integer] Only needed if MaxType IS NOT HeighestValue or AutomaticMax </p>

<p><b>DirectionType:</b> [Direction Type] Use this input to specify direction of the data bar. </p>

<p><b>GradientFill:</b> [Boolean] If set to True, generated data bar will have a gradient fill style fading from FillColor specified to White. </p>

<p><b>FillColor:</b> [Color] Color of the Data Bar</p>

<p><b>BorderColor:</b> [Color] If supplied, it will set the border color for each cell in the specified range. </p>

</blockquote>


### 3.6.2 Data Bar with Gradient no Border

In this example we highlight cells in the specified range using a gradient data bar that has no border. It also has automatic min and max values assigned that were generated based on the values in the supplied range. 

![](databar_4.png)

![](databar_2.png)

### 3.6.3 Data Bar with Border and no Gradient

In this example we highlight cells in the specified range using a data bar that has a border. It also has automatic min and max values assigned that were generated based on the values in the supplied range. 

![](databar_3.png)

![](databar_5.png)
