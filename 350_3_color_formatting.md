# 3.5.0 (3) Color Scale Formatting

(3) Color Scale Formatting allows you to set up a formatting condition that will evaluate a range of numbers and then based on some simple rules will color all of the values with an appropriate color defined in a three color gradient.

![](3color1.png)

### 3.5.1 Define Min and Max Value Types

You can define rules of how this color gradient will be applied to range of numbers by specifying Min, Mid and Max value types. This can either be as simple as "automatic" or as custom as inputting an actual number for a min/mid/max value. 

Let's have a quick look at available options and their meaning. They are very similar to onces previously discussed for the 2 Color Scale Formatting.

![](2color12png.png)

<blockquote>
<p><b> LowestValue:</b> If you chose this option, Excel will automatically chose the lowest value in the specified range and use that as a Minimum. Choosing this option means that you DO NOT have to supply MinValue. LowestValue can ONLY be applied to MinValueType input.</p>
<p><b> Number: </b> If you chose this option, you will have to also supply MinValue/MidValue/MaxValue input that will determine the minimum number. 
<p><b>Percent:</b> If you chose this option you will have to supply MinValue/MidValue/MaxValue and it will have to be between 0-100. </p>
<p><b> Formula: </b> You can use a Formula to determine a MinValue/MidValue/MaxValue. If you chose to use the formula then, you have to supply it to MinValue/MidValue/MaxValue input. Something to keep in mind when using Formulas with 3-Color Formatting is that they cannot be referencing other cells. That means that a formula like this: =1, will work just fine while something like this: =$B1=1, will not.</p>
<p><b> Percentile:</b> If you chose this option you will have to supply MinValue/MidValue/MaxValue and it will have to be between 0-100. </p> 
<p><b> HighestValue:</b> If you chose this option, Excel will automatically choose the highest value in the specified range and use that as a Maximum. Choosing this option means that you DO NOT have to supply MaxValue. HighestValue can ONLY be applied to MaxValueType input.</p>
<p><strike><b> AutomaticMax:</b> This option is NOT available for use with (2) Color Scale Formatting. </strike></p>
<p><strike><b> AutomaticMin:</b> This option is NOT available for use with (2) Color Scale Formatting. </strike></p>
<p><strike><b> None:</b> This option is NOT available for use with (2) Color Scale Formatting.</strike> </p>
</blockquote>

What this means that Lowest and Highest Value selections can only be made for Min and Max respectively. Mid value type can only be a Number, Percent, Percentile or Formula. 

### 3.5.2 Define Min and Max Values

Based on chosen Min/Max Values Types you might have to specify a numerical or formula value that will be used with this formatting style. Here's what the example above will look like:

![](3color2.png)

