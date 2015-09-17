# Consolidated Sales Report Task Pane Add-in Sample for Excel 2016

_Applies to: Excel 2016_ 

This task pane add-in shows how to consolidate data from multiple worksheets using the JavaScript APIs in Excel 2016. It comes in two flavors: text editor and Visual Studio.
![Consolidated Sales Report Sample](images/ConsolidatedSalesReport_report.png)

## Try it out
### Text editor version
1.	The simplest way to deploy and test this add-in is to copy the files to a network share. To do this, follow these steps:
	1. Create a folder on a network share (for example, \\MyShare\ConsolidatedSalesReport) and copy all the files in the Text editor folder. 
	2. Edit the <SourceLocation> element of the manifest file so that it points to the share location for the .html page from step 1. 
	3. Then copy the manifest (RangeHighlighterManifest.xml) to a network share (for example, \\MyShare\MyManifests).
	4. Then add the share location that contains the manifest as a trusted app catalog in Excel. To do this, follow these steps:
	    1. 	Launch Excel.
	    2. Choose the File tab, and then choose Options.
	    3. Choose Trust Center, and then choose the Trust Center Settings button.
	    4. 	Choose Trusted App Catalogs.
	    5. 	In the Catalog Url box, enter the path to the network share you created in Step 1, and then choose Add Catalog.
	    6. Select the Show in Menu check box, and then choose OK.
	    7. 	A message is displayed to inform you that your settings will be applied the next time you start Office. Close and restart Excel. 
        
2.	Test and run the add-in. To do this, follow these steps:
    1.  On the Insert tab in Excel 2016, choose My Add-ins. 
    2.  In the Office Add-ins dialog box, choose Shared Folder.
    3.  Choose Consolidated Sales Report Sample, and then choose Insert.
    4.  The add-in will open in a task pane to the right of the current worksheet as shown in this diagram. ![Consolidated Sales Report Sample](images/ConsolidatedSalesReport_taskpane.png)
    5. The add-in adds three new sheets with sample data for three regions, Americas, Asia, and Europe and in the task pane, it presents you with checkboxes for all of the sheets in the workbook. Select two or three of the regional data sheets and click Consolidate. You should see a new sheet called Dashboard with consolidated data from the selected sheets. ![Consolidated Sales Report Sample](images/ConsolidatedSalesReport_report.png)

### Visual Studio version
1.  Copy the project to a local folder. Then open the Excel-Add-in-JS-RangeHighlighter.sln in Visual Studio.
2. Press F5 to build and deploy the sample add-in. This will launch Excel 2016 with the add-in loaded in the task pane as shown in this diagram.  ![Consolidated Sales Report Sample](images/ConsolidatedSalesReport_taskpane.png)
3.  The add-in adds three new sheets with sample data for three regions, Americas, Asia, and Europe and in the task pane, it presents you with checkboxes for all of the sheets in the workbook. Select two or three of the regional data sheets and click Consolidate. You should see a new sheet called Dashboard with consolidated data from the selected sheets. ![Consolidated Sales Report Sample](images/ConsolidatedSalesReport_report.png)



### Learn more

This is just a sample of what can be accomplished with the new Excel JavaScript APIs. The APIs have much more to offer. If you’d like to know more, you’re welcome to explore any of the available resources. 

Here are just a few:

1.  [Excel programming guide](excel-add-ins-programming-guide.md)
2.  [Add-in code samples](excel-add-ins-code-samples.md) 
3.  [Reference](excel-add-ins-javascript-reference.md)