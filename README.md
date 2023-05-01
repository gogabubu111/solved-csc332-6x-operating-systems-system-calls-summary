Download Link: https://assignmentchef.com/product/solved-csc332-6x-operating-systems-system-calls-summary
<br>
<h2>PART 1 Simple Command Interpreter</h2>

Recall: In Task 3, we worked with exec() system calls for specific commands such as date, and ls.

Write a special simple command interpreter that takes a command and its arguments. This interpreter is a program where the main process creates a child process to execute the command using exec() family functions. After executing the command, it asks for a new command input (i.e., parent wait for child). The interpreter program will get terminated when the user enters quit.

<h2>PART 2 Average Grade Calculator</h2>

There are 10 students enrolled in a course. The course covers <em>x </em>number of chapters from a textbook (<em>x </em><em>&gt; </em>1). In each chapter <em>y </em>number of homework(s) are assigned (<em>y </em>≥ 1). The average grade for each homework in all the chapters need to be found out.

To solve this, write program which has the main process as <em>Director </em>process, which reads a file containing grades of all homeworks of all chapters and creates <em>x </em>number of <em>Manager </em>processes. Each <em>Manager </em>process will take care of solving a chapter. Each manager process will create <em>y </em>number of <em>Worker </em>process and pass one homework to each of them and they calculate and print the average.

The input file should contain the data according to the value of <em>x </em>and <em>y</em>. For example, the input text file and the process tree for <em>x </em>= 2 and <em>y </em>= 2 will look like the following:

(a)                                                                                              (b)

1

The Director process is responsible for opening and closing the input text file. It stores the values in a two dimensional integer array with 10 rows. You may need to use the following C functions (in addition to the necessary file &amp; process management system calls): fopen(), fscanf(), fseek(), fclose().


