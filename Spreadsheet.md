<table style="width:100%">
  <tr>
    <th><a href="home.md">Home</a></th>
    <th>Spreadsheets</th>
    <th><a href="OpenRefine.md">OpenRefine</a></th>
    <th><a href="RegEx.md">RegEx</a></th>.
	<th><a href="Other.md">Other</a></th>
  </tr>
</table>

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
	
</table>
