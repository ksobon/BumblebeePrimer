# 4.6.0 Top/Bottom Percentile Formatting

Top/Bottom Percentile Formatting allows you to set up a formatting condition that will either highlight a top or bottom percentile of values in a given range, or it will highlight a number of top or bottom values. 

### 4.6.1 Define Formatting Condition rules

![](topbottom_2.png)

<blockquote>
<p> 1. Equal - requires (1) value for comparison. </p>
<p> 2. NotEqual - requires (1) value for comparison. </p>
<p> 3. Greater - requires (1) value for comparison. </p>
<p> 4. GreaterEqual - requires (1) value for comparison. </p>
</blockquote>

Values can be either Strings or Numbers and it simply depends on what data you want to compare it to in Excel. For this example I will use a String. My objective is to check a range of values in Excel and determine if its equal to "Author". If it is then I want to apply a specific Graphic Style to that cell. 

### 4.6.2 Define Graphic Style

Please see section 3.0.0 for detail instructions on how to define Graphic Styles. This Graphic Style will be used if cell evaluates to True based on rules defined in previous section. 