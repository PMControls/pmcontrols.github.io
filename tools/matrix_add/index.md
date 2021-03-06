

## matrix_add

matrix_add will adds two matrices using the interface provided by LAPACK function daxpy using a scalar of 1.
The output table rows will retain the order and column names of the first input table.

After loading the smile tools, the extension function can be used with the following syntax:
```
CREATE VIRTUAL TABLE outtable 
USING matrixadd(table1 = 'tablename1', val1 = 'col1name1', val1 = 'col1name2', ..., table2 = 'tablename2', val2 = 'col2name1', val2 = 'col2name2', ...);
```
The variables are defined as follows:
- col1name1 is a column of type 'real', as is col1name2 and all subsequent columns.
- col1name1, col1name2 ... are columns of table 1.
- col2name1, col2name2 ... are columns of table 2.
- tablename1 is the name of the first table.
- tablename2 is the name of the second table.

The number of columns in tablename1 should be equal to the number of rows in tablename2.

### Usability

matrix_add is usable on all selectable real number data.

<a href="../../">home</a>
