

## matrix_transpose

matrix_transpose will transpose the columns and rows of a given input matrix.
The output table row count will be equal to the input table column count, while the output table column names will be of the format col_0, col_1, ... col_n.

After loading the smile tools, the extension function can be used with the following syntax:
```
CREATE VIRTUAL TABLE outtable 
USING matrix_transpose(table1 = 'tablename1', val1 = 'col1name1', val1 = 'col1name2', ...);
```
The variables are defined as follows:
- col1name1 is a column of type 'real', as is all subsequent columns.
- col1name1, col1name2 ... are columns of table 1.
- tablename1 is the name of the first table.

### Usability

matrix_transpose is usable on all selectable real number data.

<a href="../../">home</a>
