# table-reflow-mobile
Fork of jQuery Mobile Table Reflow widget with some UI changes and improvements.

Based on https://api.jquerymobile.com/table-reflow/

Inspired by http://doit.maryland.gov/webcom/responsivetables/responsive-tables.html

## About table reflow
The reflow table mode works by collapsing the table columns into a stacked presentation that looks like blocks of label/data pairs for each row. Since the HTML source order of a table prohibits styling a table to look like this, the plugin dynamically adds a bit of markup to make the display work (without affecting accessibility). (from jQuery Mobile web)

## Changes
Fixed text overflow if content text is longer than one row.
#### Original jQuery mobile version
![alt Original version](http://obrazky.auto-makler.cz/obrazky/table_reflow_error.png "Original version")
#### Fixed version
![alt Fixed version](http://obrazky.auto-makler.cz/obrazky/table_reflow_fix.png "Fixed version")

## Usage
To implement, ensure your tables have a <thead> and <tbody> and add the data-role="table" attribute to the table tag.

Also ensure your table has, at minimum, the "ui-responsive" class applied to it.

```html
<table class="ui-responsive" data-role="table">
  <thead>
  ...
  </thead>
  <tbody>
  ...
  </tbody>
</table>
```

```javascript
$('[data-role="table"]').reflowTable();
```
