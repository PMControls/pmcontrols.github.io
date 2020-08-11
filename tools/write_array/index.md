

## writearray

writearray is a reverse implementation of carray, from the SQLite loadable extensions library. writearray is useful for writing to c arrays, much like carray is useful for reading c arrays.

This code is intended to be used in SQLite3 to write data from a column, or set of columns, to an array. This exension function can be loaded using the following code:

```rc = sqlite3_load_extension(db, "./write_array", 0, 0);```

Where ```rc``` is a standard SQLite3 return code, and ```db``` is a pointer to a database.

The extension function can be used with the following syntax:
```
SELECT write_array($ptr, col_1, col_2, ..., col_n) from tablename;
```
The variables are defined as follows:
- $ptr is a pointer to a pointer of type double.
- col_1 is a column of type 'real', as are col_2 and all columns to col_n.
- tablename is the name of the table.

The pointer is declared prior to calling the function, and should be allocated prior to calling the function and destroyed by the calling function as well.


### Usability

writearray is usable on all selectable real number data.

<a href="../../">home</a>