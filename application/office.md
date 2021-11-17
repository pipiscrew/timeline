## Outlook

On search, **show folder** of a **mail**  

* when you have select the mail on the **listview**, press **ALT + ENTER** to get the mail properties.

Add **public holidays** to calendar by going File > Options > Calendar > there is a button `Add holidays`  

## Word
 
Merge **multiple .docx** to one  

* Select the **Insert** tab > Select **Object**, and then select **Text from File**  
* [How to merge Word documents](https://docs.microsoft.com/en-us/office/troubleshoot/word/merge-word-documents)
* [Remove Horizontal Line](https://www.howtogeek.com/217924/how-to-remove-automatic-horizontal-lines-in-word/) - go the cursor to needed line, click the table dropdown button, choose 'no border'.

## Excel
Show worksheets on a vertical list  

* Right click the left arrow that is of **left side** of **worksheets** > select **activate**  
* [Show a Vertical Worksheets List](https://www.knowledgewave.com/blog/msoffice/excel-right-click-to-show-a-vertical-worksheets-list.html)  

Vertical clipboard data to Horizontal  

* Copy the cells to **clipboard**, go to a free cell, rclick > **Paste Special** > **Transpose**  
* [Transpose option](https://www.stl-training.co.uk/b/copy-vertical-data-and-paste-it-horizontally-in-excel/)

Compare cells without vlookup, while expecting to have the same value on same line and on different column.

* Assuming we have Col A + Col B, **go to Cell C** and write the formula `=A1=B1` press **ENTER**, **expand** the formula to the **end** of cells.  

Remove blank rows  

* Home > Find & Select > Go to Special > select Blanks > ok
* now automatically selected the blank rows & columns
* Home > Delete Sheet Rows  
* [Remove blank rows](https://www.businessinsider.com/how-to-remove-blank-rows-in-excel)  

Sum selected cells  

* press ALT and =

Navigate to worksheets  

* press CTRL + PGDown / PGUp  


## See VBA (even is password protected)

* XLS
  * Open the file in a HEX editor and replace ASCII value `DPB=` with `DPx=`  
&nbsp;

* XLSX / XLSM  
1. Change the extension of the `.xlsm` file to `.zip`  
2. Extract the `xl\vbaProject.bin`  
3. Open the file in a HEX editor and replace ASCII value `DPB=` with `DPx=`
4. Double click the `xlsm` file, Excel discovers an invalid key (DPx) and asks whether you want to continue loading the project (basically ignoring the protection), `press YES!`  
5. Open the VBA editor (ALT + F11)  
6. You have to SET new password by going to Tools > 'xxx Properties' > Protection tab > enter new password  
7. press ok > CTRL + S > close EXCEL and reopen it! &nbsp; [source](https://stackoverflow.com/a/31073075)  