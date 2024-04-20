This is a copy of the meanwhile gone companion Java code by Marc Tedder
for 

M. Tedder, D. Corneil, M. Habib, and C. Paul. 
“Simpler Linear-Time Modular Decomposition Via Recursive Factorizing
Permutations”.
In: Proc ICALP 2008, https://doi.org/10.1007/978-3-540-70575-8_52

from https://web.archive.org/web/20231117180003/https://www.cs.toronto.edu/~mtedder/

In April 2023 my student Will Atherton found an error in the text,
which also shows up in the code, demostrated by a 9-vertex example
(a prime module is missing)

bug_in_tedder_example.txt


The correct (upon swapping the meanins of parallel and
serial nodes) modular decomposition of this graph can be seen by running the
code on

bug_in_tedder_example_complement.txt

Specifically, run

$ javac *.java -d .
$ java modularDecomposition/ContainsMain bug_in_tedder_example.txt
$ java modularDecomposition/ContainsMain bug_in_tedder_example_complement.txt


-------------------------------------------------------------------
- Main is contained in "ContainsMain.java".  

- The program takes a single command line argument: the name of a file specifying a graph; the comments in "Graph.java" specify the correct format for this file.  Example input files are provided by "test0.txt", "test1.txt", and "test2.txt".

- Little or no error checking is performed by the program.

- The program is still provisional in that it has not fully been tested and changes might still be made in the future.

- Thank you to Yixin Cao of the Department of Computer Science & Engineering at Texas A & M University for alerting me to a bug.

Marc Tedder (April 10, 2010)
