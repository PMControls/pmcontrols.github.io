

## plot_basic

plot_basic utilizes pbPlots to create a basic plot of input columns.

This code is intended to be used in SQLite3 to create a png file that can be stored to a table as a blob object or sent to a file using writefile(). 

The extension function can be used with the following syntax:

```
SELECT plot_basic(col_1, col_2) from tablename;
```

The variables are defined as follows:
- col_1 is a column of type 'real', and represents the x values. 
- col_2 is a column of type 'real', and represents the y values. 
- tablename is the name of the table the data is sourced from.


### Usability

plot_basic is usable on all selectable real number data.

<a href="../../">home</a>