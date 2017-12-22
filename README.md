<a href="https://github.com/gbelwariar"><img style="position: absolute; top: 0; left: 0; border: 0;" src="https://camo.githubusercontent.com/82b228a3648bf44fc1163ef44c62fcc60081495e/68747470733a2f2f73332e616d617a6f6e6177732e636f6d2f6769746875622f726962626f6e732f666f726b6d655f6c6566745f7265645f6161303030302e706e67" alt="Fork me on GitHub" data-canonical-src="https://s3.amazonaws.com/github/ribbons/forkme_left_red_aa0000.png"></a>
# Searching-and-Sorting-Library
A library containing various searching and sorting functions to search and sort a list of structures(records) according to the given comparator function.

The main objective of this project is to provide the same **flexibility** as C's qsort() in other searching and sorting algorithms. The searching and soring functions in the given library (*LIBRARY.c*) can be used for any type (including user defined types) and can be used to obtain any desired order (increasing, decreasing or any other). 

## How to use the code?

**Linux Users**

1. To generate a shared library first compile the library (*LIBRARY.c*) with the "*-fPIC*" (position independent code) flag-
***gcc -shared -o libLIBRARY.so -fPIC LIBRARY.c***.<br/>
2. Compile the sorting/searching algorithm by using the command- ***gcc FILENAME.c -ldl*** , e.g. to run the QuickSort write- ***gcc QuickSort.c -ldl***. The "*-ldl*" is used to link the dynamic library. <br/>
3. There are two fields in our structure- ID(integer type) and name(string type). Hence, pass **1** to search/sort by ID and **2** to search/sort by name, i.e- ***./a.out 1*** and ***./a.out 2*** respectively.

**Windows Users**

Since the methods like- ***dlopen()*** , ***dlsym()*** are only available in Linux, hence the above steps won't work in Windows OS.
Although one can put the functions present in the library (*LIBRARY.c*) in a header file, say- *LIBRARY.h* and then include the header in the code where those functions are to be called by adding- ***#include "LIBRARY.h"*** after setting up the proper path for the compiler to find it.

## Phases of the Projects

**1. Requirements** - Any C/C++ Compiler would work.<br/>
**2. Design** - The searching and sorting functions are kept inside a separate file (*LIBRARY.c*) to keep the design more simple.<br/>
**3. Implementation** - All projects are implemented using C.<br/>
**4. Testing/Debugging** - Several tests have been run to verify the correctness of the program. One can also find all my Test Case Generator Programs and Sample Test Cases [here](https://gbelwariar.github.io/Self-Made-Test-Case-Generators/)<br/>

## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
| [<img src="https://avatars2.githubusercontent.com/u/14831291?s=400&v=4" width="100px;"/><br /><sub>Rachit Belwariar</sub>](https://github.com/gbelwariar)<br /> | [<img src="https://avatars0.githubusercontent.com/u/17107752?s=400&v=4" width="100px;"/><br /><sub>Mazhar Imam Khan</sub>](https://github.com/MAZHARMIK)<br /> |
| :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->
