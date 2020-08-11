

## matrix_scale

matrix_scale will scale a group of columns by a given integer or double floating point value.
The output table rows will retain the order of the input table. The results of this function are similar to the following query:
```
SELECT col1*val,
       col2*val,
       ...
FROM   tablename;   
```
This function utilizes the LAPACKs dscal interface, and on its own does not provide much utility. I've included it as a test case and for possible future compatibility needs.

After loading the smile tools, the extension function can be used with the following syntax:
```
CREATE VIRTUAL TABLE outtable 
USING matrix_scale(name = 'tablename', val = 'col1name', val = 'col2name', ...);
```
The variables are defined as follows:
- col1name is a column of type 'real', as is col2name and all subsequent columns.
- tablename is the name of the table.

The pointer is declared prior to calling the function, and should be allocated prior to calling the function and destroyed by the calling function as well.

### Usability

matrix_scale is usable on all selectable real number data.
