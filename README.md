# qbtree


Task:
-----------------


There is a container for writing strings which saves them in sorted order.
The records are added and deleted all the time. In addition to that, the data
is read periodically by index number.

Need to realize a container (without multithreading) which has the following API:

 - insert a new element;
 - delete an element by index number;
 - get an element by index number;

To check the algorithm should use test data:

File write.txt - sequence of strings for origin insertion.
File modify.txt - sequence of indices for deletion and strings for insertion separated by space.
File read.txt  - sequence of indices for reading and strings for checking separated by space.

The algorithm of the test: in the container filled with data from write.txt do sequential update
(removing by index and inserting new string)  of the records from modify.txt and reading
(by specified index with checking) from read.txt .

The container must treat the dataset for a period of time not greater then 10 seconds   
(the period is real for processors with clock speed 2.26 GHz).



To build project type

cmake .
make


    ******************************************************************
    
