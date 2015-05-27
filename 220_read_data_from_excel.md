# 2.2.0 Read Data from Excel

### 2.2.1 Read Ecel

You can read Excel files in a number of different ways using Bumblebee. You can read an entire sheet contents, read from specified origin point, read only a specific range of data or do all of the former but for multiple sheets. Let's start with some basic reading set up: 

![](readExcel.png)

<blockquote>
<p><b> FilePath:</b> [FilePath] Use FilePath node to point at Excel file that you wish to read data from. </p>

<p><b> RunIt:</b> [Boolean] Set this to True to enable this node and read data from file. Set this to False to disable this node. </p>

<p><b> SheetName:</b> [String or List[String]] Set this input to a single sheet name or use a list of sheet names to read multiple sheets.</p>

<p><b> ByColumn:</b> [Boolean] Set this input to True to read excel data "by column" instead of default excel behavior "by row" </p>

<p><b> Origin:</b> [String or List[String]] Leave this input blank and default origin is set to start at A1. You can either supply an excel address format: "A1" or a cell index format List[1,1] to set the origin cell from which data will be read </p>

<p><b> Extent:</b> [String or List[String]] Leave this input blank and default extent is set to read the whole sheet. You can either supply an excel address format: "A13" or a cell index format List[1,13] to constrain the extent of document that you want to read.</p>

</blockquote>