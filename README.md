## SMiLe (SQLite extension collection)

SMiLe is a set of lightweight data analysis tools intended for SQLite. SMiLe tools can be compiled with SQLite source code, or loaded at runtime using SQLite's .load syntax. The tools are written in c, and often include Python scripts to provide example utilizations of the tools. In general, a full-featured data analysis toolset such as those provided by R and Python will be a preferrable option. For those cases where you just need a self-contained, portable system capable of self-analysis, you may find SMiLe to be suitable for your needs.

The github SMiLe library is new, and for now only includes write_array.c and supporting files. Feel free to drop comments or criticisms of the work so far. Thanks for stopping by. 

### Goals

Currently SMiLe goals are focused on providing simple analysis operations. These operations are in proof-of-concept phase. Please do not attempt to use this code in production work.

### SQLite

SQLite is a fast, easy database solution. You can find out much more about SQLite at https://www.sqlite.org/index.html

### pbPlots

pbPlots is used to generate aggregate plots. pbPlots provides an extensive range of plotting functions, and you can find more about pbPlots here: https://github.com/InductiveComputerScience/pbPlots

### CLAPACK

SMiLe utilizes a non-optimized subset of the CLAPACK library. You can find a full version of CLAPACK at www.netlib.org/clapack

### Tools:

writearray.md <a href="writearray.md">writearray</a>
