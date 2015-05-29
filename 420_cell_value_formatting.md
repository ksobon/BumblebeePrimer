# 4.2.0 Cell Value Formatting

Cell Value Formatting allows you to set up a formatting condition that relies on a value that is contained within each cell that formatting is applied to. This basically allows you to compare each cell to some value and based on some simple comparison operators like "equals" or "less than" you can apply certain style to cell based on that comparison result. 

### 4.2.1 Choose Operator Type and Values

![](cellValue1.png)

Based on what Operator Type you chose, you will either have to supply one or more values that each cell will be evaluated against. Operator Types available are pretty straight forward and are mostly similar to some of the logical operators that you have already seen in Excel: 

![](cellValue2.png)

<blockquote>
<p> 1. Equal - requires (1) value for comparison. </p>
<p> 2. NotEqual - requires (1) value for comparison. </p>
<p> 3. Greater - requires (1) value for comparison. </p>
<p> 4. GreaterEqual - requires (1) value for comparison. </p>
<p> 5. Less - requires (1) value for comparison. </p>
<p> 6. LessEqual - requires (1) value for comparison. </p>
<p> 7. Between - requires (2) values for comparison. </p>
<p> 8. NotBetween - requires (2) values for comparison. </p>
</blockquote>

Values can be either Strings or Numbers and it simply depends on what data you want to compare it to in Excel. For this example I will use a String. My objective is to check a range of values in Excel and determine if its equal to "Author". If it is then I want to apply a specific Graphic Style to that cell. 

You can either use a Code Block or a String Node like so:

![](cellValue3.png)

Once we have our condition defined we can move on to defining Graphic Style that will be applied to cells that evaluate to True for the given condition. 

### 4.2.2 Define Graphic Style

Please see section 3.0.0 for detail instructions on how to define Graphic Styles.

### 4.2.4 Define Text Style

![](textStyle.png)

<blockquote>
<p><b> Name:</b> [String] This input has to be a name of a font that is currently installed on your machine.</p>
<p><b> Size:</b> [String] Please specify a size of font to be used as a String. For example: "12" and NOT 12 which would be an integer.</p>
<p><b> FontColor:</b> [Color] If you wish to specify different than black font color use Color.ByARGB node to do so.</p>
<p><b> HorizontalAlignType:</b> [Horizontal Align Type] This can be set to Left, Center or Right. </p>
<p><b> VerticalAlignType:</b> [Vertical Align Type] This can be set to Top, Middle or Bottom. </p>
<p><b> Bold:</b> [Boolean] Set it to True for font to be bold. </p>
<p><b> Italic:</b> [Boolean] Set it to True for font to be italic.</p>
<p><b> Underline:</b> [Boolean] Set it to True for font to have an underline.</p>
<p><b> Strikethrough:</b> [Boolean] Set it to True for font to have a strikethrough.</p>
</blockquote>

### 4.2.5 Define Border Style

![](borderStyle.png)

<blockquote>
<p><b> LineType:</b> [Line Type] If you wish to define a line type different than a solid use this input to do so.</p>
<p><b> LineWeightType:</b> [Line Weight Type] Line weights can only be one of the following types: Hairline, Medium, Thick or Think.</p>
<p><b> LineColor:</b> [Color] If you wish to specify line color use Color.ByARGB node to do so.</p>
</blockquote>

### 4.2.6 Cell Value Format Condition - Single Range/Single Format Condition

![](cellValue6.png)

This is what the final result will look like:

![](cellValue8.png)

### 4.2.7 Cell Value Format Condition - Single Range/Multiple Format Conditions

You can also stack more than one Format Condition on top of each other and formatting will be applied based on order that they were added in case that both Format Conditions evaluate to True. Here's an example:

![](cellValue9.png)

This is what the final result will look like:

![](cellValue10.png)

### 4.2.8 Cell Value Format Condition - Multiple Ranges/Multiple Format Conditions

You can also apply different Format Conditions to more than one range at the time while maintaining ability to add more than one Format Condition per Range. Just create lists of lists of Format Conditions and you will be good to go. 

![](cellValue11.png)

This is what the final result will look like:

![](cellValue12.png)

The trick is to match the length of the Cell Range list with the Format Conditions list like so: 

![](cellValue13.png)
