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

Please see section 3.0.0 for detail instructions on how to define Graphic Styles. This Graphic Style will be used if cell evaluates to True based on rules defined in previous section. 

### 4.2.3 Cell Value Format Condition - Single Range/Single Format Condition

![](cellValue6.png)

This is what the final result will look like:

![](cellValue8.png)

### 4.2.4 Cell Value Format Condition - Single Range/Multiple Format Conditions

You can also stack more than one Format Condition on top of each other and formatting will be applied based on order that they were added in case that both Format Conditions evaluate to True. Here's an example:

![](cellValue9.png)

This is what the final result will look like:

![](cellValue10.png)

### 4.2.5 Cell Value Format Condition - Multiple Ranges/Multiple Format Conditions

You can also apply different Format Conditions to more than one range at the time while maintaining ability to add more than one Format Condition per Range. Just create lists of lists of Format Conditions and you will be good to go. 

![](cellValue11.png)

This is what the final result will look like:

![](cellValue12.png)

The trick is to match the length of the Cell Range list with the Format Conditions list like so: 

![](cellValue13.png)
