# First In First Out Page Replacement Algorithm - FIFO
This is an implementation of the First In First Out (FIFO) page replacement algorithm.

## Overview
This is a C program that implements the First In First Out (FIFO) page replacement algorithm. The program reads a file containing a list of memory references, and simulates how the memory management system would operate with a given number of physical pages and page size.

The program calculates the number of page faults for a sequence of memory references (i.e., the
memory reference trace in the .mem-files) when using the FIFO (First-In-First-Out) page replacement policy.
The program takes the number of physical pages, the page size, and the name of the trace file:
```sh
./fifo no_phys_pages page_size filename
```

The program then returns the resulting number of page faults for that specific combination of number of pages and page size,
for either mp3d.mem or mult.mem.
Example execution:
```sh
mycomputer$ ./fifo 4 256 mp3d.mem
No physical pages = 4, page size = 256
Reading memory trace from mp3d.mem... Read 100000 memory references
Result: 11940 page faults
```

## Usage
To use this program, you need to provide three arguments: the number of physical pages, the page size, and the name of the file containing the memory references. For example:
