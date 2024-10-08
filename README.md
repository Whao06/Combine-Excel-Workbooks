# Combine-Excel-Workbooks
This program will combine multiple Excel files or csv files together into a single Excel workbook. It will also delete any empty sheets with no data.<br>
<h2>Merging Excel Files into One Excel File</h2>
1. Prepare a new text file with the name <b>table-list</b> and have the path of the excel files that need to be merged as shown below:
<br><br>
<p align = "center">   
<img src="https://github.com/Whao06/Combine-Excel-Workbooks/blob/main/Excel.PNG" alt="Example">
</p>
<br>
3. In a new excel file, press <b>ALT + F11</b> to open Visual Basic Editor. <br>
4. Right-click <b>ThisWorkbook</b> and select insert module. <br>
5. Use the code at <b>merge.xlsm</b>. <br>
6. Press <b>CTRL + S</b> and save as <b>Excel macro-enabled workbook</b>. <br>
7. Press <b>"NO"</b> if there is warning dialog. <br>
8. Close Visual Basic Editor. <br>
9. In the excel file, press <b>ALT + F8</b> to see the Macro Window. <br>
10. Select and run the merging macro. <br>
11. Click <b>Delete</b> until the pop-up window disappear. <br>

<h2> Notes </h2>
1. The <b>DELETE</b> function will remove empty sheets with no data inside.<br>
2. You can add the following code under <b>"This Workbook"</b> to have the macro run everytime you open the excel file:<br>

```
Private Sub Workbook_Open()
    Call MergeExcelFiles
End Sub
```
<h2>References</h2>
<ul>
        <li>https://www.ablebits.com/office-addins-blog/merge-multiple-excel-files-into-one/ </li>
        <li>https://github.com/tinyheero/merge-excel-workbooks</li>
</ul>

