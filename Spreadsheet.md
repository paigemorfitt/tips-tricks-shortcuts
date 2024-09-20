<table style="width:100%">
  <tr>
    <th><a href="home.md">Home</a></th>
    <th>Spreadsheets</th>
    <th><a href="OpenRefine.md">OpenRefine</a></th>
    <th><a href="RegEx.md">RegEx</a></th>.
	<th><a href="Other.md">Other</a></th>
	<th><a href="Acronyms.md">Acronyms</a></th>
	<th><a href="Glossery.md">Glossery</a></th>
  </tr>
</table>
	<h4>Note: Due to changes in Excel (the change from letters to numbers for column labeling) these exact equations will need to be tweaked (4/12/2024)</h4>
<table>
	<tr>
		<th>Where</th>
		<th>What</th>
		<th>Equation</th>
		<th>Explanation</th>
		<th>Example</th>
		<th>Date Checked</th>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>to find and count any findings of that text in a cell</td>
		<td>=countIf(B3, "*(Sh)Review*")</td>
		<td>Looks in B3 and counts if it finds any "(Sh)Review" in that cell</td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=3:3"</a>Example (Row 3)</td>
		<td>November 2023</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>to count all "False" statements and identify what that number indicates</td>
		<td>="Un-Suppressed : "&(countif(B4:G4, False))</td>
		<td>Create a True/False situation in Column B. This will only count 
		"False"</td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=4:4"</a>Example (Row 4)</td>
		<td>November 2023</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>to change all caps in a cell</td>
		<td>=proper(B1)</td>
		<td></td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=5:5"</a>Example (Row 5)</td>
		<td>January 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Adds hyperlink to a if/then statement based on term</td>
		<td>=if(A6="Don't know",HYPERLINK("https://www.merriam-webster.com/dictionary/don%27t%20know", "I don't know (for help)"), if(A6="Yes", "Fix in spreadsheet", if(A6="No", "Skip Columns D-E", "")))</td>
		<td></td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=6:6"</a>Example (Row 6)</td>
		<td>February 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>count all characters in a cell</td>
		<td>=len(A3)</td>
		<td></td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=7:7"</a>Example (Row 7)</td>
		<td>February 2024</td>
	</tr>
	 <tr>
		<td>Google Sheets</td>
		<td>highlight cell based on cell value</td>
		<td>=countif(F:F,F:F)>1</td>
		<td>Highlights all cells in Column F that have duplicate values in column F</td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=1566302292&range=B:D"</a>Example (Column B-D)</td>
		<td>March 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Indicates if cells from B9-G9 match what is in column F</td>
		<td>=countif(B9:G9,F:F)>1</td>
		<td>Highlights all cells in Column F that have duplicate values in column F</td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=8:8"</a>Example (Row 8)</td>
		<td>March 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Helps create alphabet</td>
		<td>=CHAR(CODE(A1) + 1)</td>
		<td>Add "A" in the first cell, then put equation in the next, and it will insert a "B". Drag to add more letters. </td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=9:9"</a>Example (Row 9)</td>
		<td>April 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Conditional format check</td>
		<td>=if(AND (B25=0, B30=0, B20=0, B15=0, B10=0), "Yes", "No")</td>
		<td>Conditional format that indicates if all indicated cells equal "1" then "Yes"</td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=10:11"</a>Example (Rows 10-11)</td>
		<td>April 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Replaces one word for another</td>
		<td>=SUBSTITUTE(A2, "at", "ate") </td>
		<td> </td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=12:12"</a>Example (Row 12)</td>
		<td>April 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Imports live table from website</td>
		<td>=importhtml("https://en.wikipedia.org/wiki/Hans_Zimmer_discography", "Table", 1)</td>
		<td>Equation imports Table 1 found on Hanz Zimmer's discography wikipedia page. </td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=1566302292&range=F:J"</a>Example (Column F-J)</td>
		<td>April 2024</td>
	</tr>
	<tr>
		<td>Google Sheets</td>
		<td>Joins a group of cells in the range B13 to G13 and uses "-" as the joining character</td>
		<td>=JOIN("-",B13:G13)</td>
		<td>For Excel, use TEXTJOIN("-",TRUE, B13:G13). TESTJOIN also works in Sheets</td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=13:13"</a>Example (Row 13)</td>
		<td>April 2024</td>
	</tr>
	<tr>
		<td>Excel</td>
		<td>Looks up the value of A2 in the spreadsheet tab "Sheet1 Column B then upon match, imports from the same tab the corresponding column A</td>
		<td>=XLOOKUP(A2, Sheet1!B:B, Sheet1!A:A)</td>
		<td>This works with tabs within the same spreadsheet</td>
		<td>N/A</td>
		<td>September 2024</td>
	</tr>
	<tr>
		<td>Google Sheets & Excel</td>
		<td>Looks up Value in Cell C14 in tab 'Sheet3' column K. If it is found, it will display content from column L for that cell value</td>
		<td>XLOOKUP(C14,Sheet3!K:K,Sheet3!L:L)</td>
		<td>This is for working within the same spreadsheet. </td>
		<td><a href="https://docs.google.com/spreadsheets/d/1Rmushce4Gin2e-RcT-JL_NJg54GWb5fxofzF4mGpO5Q/edit#gid=0&range=14:14"</a>Example (Row 14)</td>
		<td>September 2024</td>
	</tr>
		<tr>
		<td>Google Sheets</td>
		<td>Looks up Value in Cell F2 in spreadsheet 'https://docs.google.com/spreadsheets/d/1R8qQFtq6lmGVkXyDV3jdNX5SD_AVHBH9_FI4kTGCuiU/edit?gid=545735534#gid=545735534''s tab 
'Scores @ Music Library' column A. If it is found, it will display content from 'https://docs.google.com/spreadsheets/d/1R8qQFtq6lmGVkXyDV3jdNX5SD_AVHBH9_FI4kTGCuiU/edit?gid=545735534#gid=545735534''s tab 
'Scores @ Music Library' column AM</td>
		<td>xlookup(F2,IMPORTRANGE("https://docs.google.com/spreadsheets/d/1R8qQFtq6lmGVkXyDV3jdNX5SD_AVHBH9_FI4kTGCuiU/edit?gid=545735534#gid=545735534","Scores @ Music Library!a1:a"),IMPORTRANGE("https://docs.google.com/spreadsheets/d/1R8qQFtq6lmGVkXyDV3jdNX5SD_AVHBH9_FI4kTGCuiU/edit?gid=545735534#gid=545735534","Scores @ Music Library!m1:m"))</td>
		<td>xlookup(F2,IMPORTRANGE("[link to second spreadsheet you are working with]","[Tab name from that spreadsheet you are looking in]![Column where the value of "F" is in the second spareadsheet]"),IMPORTRANGE("[link to second spreadsheet you are working with]","[Tab name from that spreadsheet you are looking in]![Column you want to add to your first spreadsheet]"))</td>
		<td>N/A</td>
		<td>September 2024</td>
	</tr>
		<tr>
		<td>Google Sheets</td>
		<td>Add date to spreadsheet</td>
		<td>CTRL + ;</td>
		<td>N/A</td>
		<td>N/A</td>
		<td>September 2024</td>
	</tr>
				</tr>
		<tr>
		<td>Google Sheets</td>
		<td>Add time to spreadsheet</td>
		<td>CTRL + Shift + ;</td>
		<td>N/A</td>
		<td>N/A</td>
		<td>September 2024</td>
	</tr>
</table>
