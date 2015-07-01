# 4.2.0 Clear Contents

Clear Contents is a node that will allow you to do few things. One of them is to clear data or cell content from a range of Excel sheet. It can also clear any formatting applied to those cells (color fills, text style overrides etc.). 

####There is only one rule here: please close Excel when trying to override a file. :-)

![](clearContent.png)

### 4.2.1 Set up

<blockquote>
<p><b> FilePath:</b> [File Path] Use FilePath node to point at Excel file that you wish to read data from.</p>
<p><b> RunIt:</b> [Boolean] Set this to True to enable this node and read data from file. Set this to False to disable this node.</p>
<p><b> SheetName:</b> [String] Set this input to a single sheet name or use a list of sheet names to read multiple sheets.</p>
<p><b> ClearContent:</b> [Boolean] If set to True all Cell Content will be removed. This means that data contained inside of cells which includes formulas will be deleted.</p>
<p><b> ClearFormatting:</b> [Boolean] If set to True all formatting for specified range will be cleared. Formatting constitutes of things such as Cell Fills or Text Styles. </p> 
<p><b> Range:</b> [String] An Excel Range in format: "A1:B10" that if supplied will apply clear functions only to range specified. If this input is empty clear funtions will be applied over entire document.</p>

</blockquote>