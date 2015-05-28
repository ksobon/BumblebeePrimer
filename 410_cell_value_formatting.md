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

While defining Graphic Style you can chose to either override one or all of the available styles. If you wish to not override Border Style then just leave that input empty.

![](cellValue4.png)

<blockquote>
<p><b> FillStyle:</b> [Fill Style] If you supply a fill style to this input it will be overriden to whatever fill style settings were defined for that fill style.</p>
<p><b> TextStyle:</b> [Text Style] If you supply a text style to this input it will be overridden to whatever text style settings were defined for that text style.</p>
<p><b> BorderStyle:</b> [Border Style] If you supply a border style to this input it will be overridden to whatever border style settings were defined for that text style.</p>
</blockquote>

### 4.2.3 Define Fill Style

![](cellValue5.png)

<blockquote>
<p><b> PatternType:</b> [Pattern Type] If you wish to apply fill pattern to a cell use this input to specify it.</p>
<p><b> BackgroundColor:</b> [Color] If you wish to specify a background color in a cell use Color.ByARGB node to do so.</p>
<p><b> PatternColor:</b> [Color] If you wish to specify pattern color use Color.ByARGB node to do so.</p>
<p><b> Bevel:</b> [Bevel Type] Currently unavailable </p>
<p><b> Opacity:</b> [Integer] Currently unavailable </p>
</blockquote>

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
