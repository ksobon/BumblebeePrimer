# 4.1.0 Conditional Formatting Overview

Conditional Formatting in Excel can be a really powerful tool. If you ever wanted to use Excel as a model checking or model management tool on Revit projects then this will come really handy for you. I use it to extract all kinds of data and parameters and then apply conditional formatting to it to quickly identify mistakes and imissions. Let's first have a look at how the main conditional format node is set up and we can go from there:

### 4.1.1 Set Up

![](conditionalFormat1.png)

<blockquote>
<p><b> FilePath:</b> [FilePath] Use this input to specify excel file that formatting will be applied to. </p>

<p><b> RunIt:</b> [Boolean] Set this input to True to enable this node and execute it. Set it to False to disable it. </p>

<p><b> SheetName:</b> [String] Use this input to specify what sheet you want to apply the formatting to. </p>

<p><b> CellRange:</b> [String or List[String]] Use this node to define a specific range that you want the formatting to be applied to. Typical Excel syntax applies where range is defined like so: "A1:B1". </p>

<p><b> FormatConditions:</b> [FormatCondition or List[FormatCondition]] Use this input to supply a single Format Condition object (for example a Cell Value FC) or a list of multiple Format Conditions. This allows you to combine multiple Cell Value format conditions or apply them to multiple ranges. 
</blockquote>

### 4.1.2 Example:

Multiple Formatting Conditions applied to multiple ranges in an Excel file helping me identify parameters in my Drawing List that were not set or set incorrectly. 

![](conditionalFormat2.png)

Rules Box in Excel that reflects all of the Conditions applied. 

![](conditionalFormat3.png)

