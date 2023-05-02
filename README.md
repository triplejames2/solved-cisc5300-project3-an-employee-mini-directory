Download Link: https://assignmentchef.com/product/solved-cisc5300-project3-an-employee-mini-directory
<br>



<strong>Programming Project #5</strong>

Let’s build a mini-directory that allows us to look up employee information. Your program will first read this information from a data file, after which it will display all the data that was input. Next, your program will repeatedly query the user for a employee’s name, display the each employee’s information. To keep things simple, let’s only track an employee’s name, office, and phone extension.

To do this cleanly, let’s use a Minidir datatype for mini-directories. This datatype should be designed as a class having the following member functions:

<ul>

 <li>is_empty(), whose value is true if the Minidir object is empty, and false otherwise.</li>

 <li>find(), which finds an employee with a particular name, that name being a string parameter.</li>

</ul>

The implementation data of a Minidir will be a vector&lt;Employee&gt;, called data. This data should be private, since we don’t want a query program to change our database.

Minidir will also have two helper functions: an input operator and an output operator. These will be friends of the Minidir class, meaning that they can access data, even they’re not member functions.

Note that we have now introduced an Employee datatype. Let’s implement this as a struct having data members named name, office, and phone, all of which should be strings. This datatype will also have an input operator and an output operator as helper functions. I found it helpful to also have a three-parameter constructor, the parameters being the name, office, and phone number. Not surprisingly, the Minidir datatype will be given by two files:

<ul>

 <li>h: the header file for the Employee and Minidir datatypes.</li>

 <li>cc: the corresponding implementation file.</li>

</ul>

In addition, you’ll need a file proj5.cc, whose main function reads a mini-directory from an input file, prints the whole directory on standard output, and then goes into a query/response loop allowing the user to look up employee information.

The project share directory ~agw/class/programming-c++/share/proj5 contains the following files:

<ul>

 <li>A header file Minidir.h for the class.</li>

 <li>A stub version proj5-stub.cc of proj5.cc.</li>

 <li>A working Linux executable proj5-agw that you can play around with.</li>

 <li>A Makefile, so that you can use make to build the program and make clean to clean up detritus.</li>

</ul>

Copy these to your working directory, as usual.

Your job is to flesh out the details of proj5.cc and to write the implementation file Minidir.cc. Please work incrementally.

<strong>Deliverables: </strong>A clean typescript, consisting of the following lines and their output:

cat Minidir.cc cat proj5.cc make clean make proj5 data0 proj5 data1 proj5 data2