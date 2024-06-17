<table style="width:100%">
  <tr>
    <th><a href="home.md">Home</a></th>
    <th><a href="Spreadsheet.md">Spreadsheets</a></th>
    <th>OpenRefine</th>
    <th><a href="RegEx.md">RegEx</a></th>
	<th><a href="Other.md">Other</a></th>
	<th><a href="Acronyms.md">Acronyms</a></th>
  </tr>
<table>
<table>
	<tr>
		<th>Action</th>
		<th>What</th>
		<th>Equation</th>
		<th>Explanation</th>
		<th>From this</th>
		<th>To this</th>
		<th>Date Checked</th>
	</tr>
	<tr>
		<td>Edit</td>
		<td>First, repalce every "," with a ":", then remove everything after the ";"</td>
		<td>value.replace(/\,.*/,';')</td>
		<td>The ";" remains at the end</td>
		<td>	Bioterrorism, Bioterrorism—Health aspects, Disaster medicine, Terrorism—Prevention</td>
		<td>Bioterrorism;</td>
		<td>February 2024</td>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Reformats dates from Month to Number</td>
		<td>value.split(" ").reverse().join("-").replace('January','01-').replace('February','02-').replace('March','03-').replace('April','04-').replace('May','05-').replace('June','06-').replace('July','07-').replace('August','09-').replace('September','09-').replace('October','10-').replace('November','11-').replace('December','12-').replace('Spring','21-').replace('Winter','24-').replace('Summer','22-').replace('Fall','23-')</td>
		<td>Still needs clean up/individual intervention for complex dates</td>
		<td>Spring 1978</td>
		<td>1978-21-</td>
		<td>February 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Reformats abbreviated months to spelt out month</td>
		<td>value.replace('Jan','January').replace('Feb','February').replace('Mar', 'March').replace('Apr', 'April').replace('Jun', 'June').replace('Jul', 'July').replace('Aug', 'August').replace('Sept', 'September').replace('Sep', 'September').replace('Oct', 'October').replace('Nov', 'November').replace('Dec', 'December')</td>
		<td></td>
		<td>Oct 1902-Jun 1903</td>
		<td>October 1902-June 1903</td>
		<td>February 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Reformats leading '0' in display date</td>
		<td>value.replace(' 01,',' 1,').replace(' 02,',' 2,').replace(' 03,',' 3,').replace(' 04,',' 4,').replace(' 05,',' 5,').replace(' 06,',' 6,').replace(' 07,',' 7,').replace(' 08,',' 8,').replace(' 09,',' 9,')</td>
		<td>Remove "0" from "August 01, 2019")</td>
		<td>March 02, 1926</td>
		<td>March 2, 1926</td>
		<td>February 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Filter</td>
		<td>Filters by tells that have "T"</td>
		<td>value.contains("T")</td>
		<td>Capitalization matters</td>
		<td>N/A</td>
		<td>N/A</td>
		<td>February 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Replaces "unknown" with "?"</td>
		<td>replace(value, "unknown" , "?")</td>
		<td></td>
		<td>unknown/1910</td>
		<td>?/1910</td>
		<td>February 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Split value by " "(space), reverse order, join again by "-"</td>
		<td>value.split(" ").reverse().join("-")</td>
		<td>When you have multiple split values, it gets messy. </td>
		<td>May 1892</td>
		<td>1892-May</td>
		<td>February 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Add text before cell content</td>
		<td>"Abstract Type: " + cells["abstract_format"].value</td>
		<td>This adds the text "Abstract Type: " to the beginning of all content in the column "abstract_format"</td>
		<td>html</td>
		<td>Abstract Type: html</td>
		<td>April 2024</td>
	</tr>
	</tr>
		<tr>
		<td>Edit</td>
		<td>Add text after cell content</td>
		<td>cells["abstract_format"].value + " (form of abstract)"</td>
		<td>This adds the text  (form of abstract) to the end of all content in the column "abstract_format"</td>
		<td>html</td>
		<td>html (form of abstract)</td>
		<td>April 2024</td>
	</tr>
</table>
