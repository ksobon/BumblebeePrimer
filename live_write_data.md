# 1.3.0 Write Data to Excel in Live Mode

Given large community outcry (yes, I am looking at you - Shane Burger) I decided to include this node in Bumblebee. It will allow you to stream data to Excel while Excel is open and results will display/update in Excel instantly - or as fast as it takes Excel to refresh. 

#### One rule here is to have ONLY the document that you intend to override open, since this node will write to first Excel file that it encounters in the ROT (Running Objects Table). 

### 1.2.1 Write Multiple Rows of Data to Excel

This is probably the most common application for Bumblebee - writing a nested list of data to multiple columns or rows to an Excel spreadsheet. Here's how its done: 

![](image01.png)

<blockquote>

<p><b>RunIt:</b> [Boolean] If set to False it will disable this node. If set to True it will enable this node and execute the write process.</p>

<p><b>ByColumn:</b> [Boolean] If set to False this file will be written "By Row" which is a standard Excel writing method. Setting it to True will be equivelant to performing a Transpose function on data before writing it.</p>

<p><b>BBData:</b> [BBData] This is a BBData input. Please see below for how this node can be set up.</p>
</blockquote>