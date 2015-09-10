##Geekwise Introduction to `<HTML>` and `CSS`
###Thursday
###Date: 09-10-2015

##Overview
### 1: Review important concepts from the prior day
* Tables,tables,tables!
* Permisions and sharing a live webpage on your Geekwise Google Drive account.

### 2: Share an overview of what will they will learn today
* Continue expand on using tables for creating and interacting with structured data.
* Using tables for our weekly team webpage.

### 3: Practice exercise related to concept and objective
* Working on completing the 3 page `website` with the following pages
* Home | About | Contact
* Using tables to create structured data for our 3 page `website`


### 4: Closing session and circling back to objective of the day
* Tables are import for sharing sturctured data.
## * Creating a full 3 page `HTML` site using `.html` files with table content.

---
#Reference

#Tables

Tag       |Code
----------|---------------------------------|
table     |`<table>Places a table on your page</table>`
caption   |`<caption>caption of the table</caption>`
tr        |`<tr>starts a new table row. Cells go inside this</tr>`
td        |`<td>A cell containing actual data. Encloses a table cell. Content goes in these</td>`
th        |`<th>same as table cells, but with all contents bold and aligned to the center</th>`
thead     | `<thead>Defines the header part of a large table. Wrap the tags around the rows/cells you wish to define as the header.</thead>`
tbody     |`<tbody>It is always worth using this tag, as well as using <thead> and <tfoot> where appropriate.</tbody>`
tfoot     |`<tfoot>Good place to put summary data, such as totals. Note that it goes before the <tbody> tag!</tfoot>`
col       | `<col>Identifies a particular column in a table. can be applied to each first column in a series of tables, then the width of each column may be set to be equal in the stylesheet, overriding the table’s natural tendency to adjust its own column widths to fit its contents.</col>`
colgroup  |`<colgroup>Allows you to set attributes for the entire column. Each column has to be defined sequentially</colgroup>`

---

> You are able to have more than one table head,body and footer per table.

#Table Examples 1:

<table>
  <caption>Types Of Citrus Fruit</caption>
	<colgroup span="2" class="columns1and2"></colgroup>
	<tr>
		<th>lime</th>
		<th>lemon</th>
		<th>orange</th>
		<th>grape fruit</th>
	</tr>
	<tr>
		<td>8</td>
		<td>7</td>
		<td>12</td>
		<td>5</td>
	</tr>
</table>

```
<table>
  <caption>Types Of Citrus Fruit</caption>
	<colgroup span="2" class="columns1and2"></colgroup>
	<tr>
		<th>lime</th>
		<th>lemon</th>
		<th>orange</th>
		<th>grape fruit</th>
	</tr>
	<tr>
		<td>8</td>
		<td>7</td>
		<td>12</td>
		<td>5</td>
	</tr>
</table>
```

#Table Example 2:

<table>
	<thead>
		<tr>
			<th>Header 1</th>
			<th>Header 2</th>
			<th>Header 3</th>
		</tr>
	</thead>
	<tfoot>
		<tr>
			<td>Footer 1</td>
			<td>Footer 2</td>
			<td>Footer 3</td>
		</tr>
	</tfoot>
	<tbody>
		<tr>
			<td>Cell data 1</td>
			<td>Cell data 2</td>
			<td>Cell data 3</td>
		</tr>
		<tr>
			<td>Cell data 4</td>
			<td>Cell data 5</td>
			<td>Cell data 6</td>
		</tr>
		<tr>
			<td>Cell data 7</td>
			<td>Cell data 8</td>
			<td>Cell data 9</td>
		</tr>
	</tbody>
</table>

```
<table>
	<thead>
		<tr>
			<th>Header 1</th>
			<th>Header 2</th>
			<th>Header 3</th>
		</tr>
	</thead>
	<tfoot>
		<tr>
			<td>Footer 1</td>
			<td>Footer 2</td>
			<td>Footer 3</td>
		</tr>
	</tfoot>
	<tbody>
		<tr>
			<td>Cell data 1</td>
			<td>Cell data 2</td>
			<td>Cell data 3</td>
		</tr>
		<tr>
			<td>Cell data 4</td>
			<td>Cell data 5</td>
			<td>Cell data 6</td>
		</tr>
		<tr>
			<td>Cell data 7</td>
			<td>Cell data 8</td>
			<td>Cell data 9</td>
		</tr>
	</tbody>
</table>
```

#Table Example 3:
<table>
	<tr>
		<th>Question</th>
		<th>Answer</th>
		<th>Correct?</th>
	</tr>
	<tr>
		<td>What is the capital of Burundi?</td>
		<td>Bujumburra</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>What is the capital of France?</td>
		<td>F</td>
		<td>Erm... sort of</td>
	</tr>
</table>
```
<table>
	<tr>
		<th>Question</th>
		<th>Answer</th>
		<th>Correct?</th>
	</tr>
	<tr>
		<td>What is the capital of Burundi?</td>
		<td>Bujumburra</td>
		<td>Yes</td>
	</tr>
	<tr>
		<td>What is the capital of France?</td>
		<td>F</td>
		<td>Erm... sort of</td>
	</tr>
</table>
```


#Table Example 4 (centered and responsive):

```
<html>
<title>Centered and Responsive Table Date</title>
<head>
	<style>
	table { 
	  width: 100%; 
	  border-collapse: collapse; 
	}
	tr:nth-of-type(odd) { 
	  background: #eee; 
	}
	th { 
	  background: #333; 
	  color: white; 
	  font-weight: bold; 
	}
	td, th { 
	  padding: 6px; 
	  border: 1px solid #ccc; 
	  text-align: left; 
	}
	</style>
</head>
<body>
	
	
	
	<table>
		<thead>
		<tr>
			<th>First Name</th>
			<th>Last Name</th>
			<th>Class Name</th>
		</tr>
		</thead>
		<tbody>
		<tr>
			<td>Roger</td>
			<td>Chang</td>
			<td>Javascript Application Development</td>
		</tr>
		<tr>
			<td>Eric</td>
			<td>Cesena</td>
			<td>Javascript Application Development</td>
		</tr>
		</tbody>
	</table>

</body>
</html>
```