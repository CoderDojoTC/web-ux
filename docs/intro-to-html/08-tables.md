# HTML Tables
Tables allow us to place content in regular rows and columns within a region of a page.  Tables can be used to place text into two columns to make it easer to read, but they can also be used to create complex displays of reports that include header descriptions and footer totals.

We will start with a simple description of a table and then build a more detailed example.

## Creating a Simple Table: Two Column Layout
Here is a simple example of using a table to place text into two vertical columns.  We will use both a ```<tr>``` element for a table row and a ```<td>``` element for the table data.

```html
<table>
   <tr>
      <td>This text will be placed into the left column 1</td>
      <td>This text will be placed into the right column 2</td>
  </td>
</table>
```

Here is how this table will render on a web page:

<table>
   <tr>
      <td>This text will be placed into the left column 1</td>
      <td>This text will be placed into the right column 2</td>
  </td>
</table>

## A Table with Header and Footer elements

```
<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Mentors</th>
      <th>Students</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>4</td>
      <td>12</td>
    </tr>
    <tr>
      <td>February</td>
      <td>5</td>
      <td>15</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>March</td>
      <td>6</td>
      <td>24</td>
    </tr>
  </tfoot>
</table>
```

<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Mentors</th>
      <th>Students</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>4</td>
      <td>12</td>
    </tr>
    <tr>
      <td>February</td>
      <td>5</td>
      <td>15</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>March</td>
      <td>6</td>
      <td>24</td>
    </tr>
  </tfoot>
</table>
