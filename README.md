Download Link: https://assignmentchef.com/product/solved-cis-212-assignment-5-data-from-a-file
<br>
The goal of this assignment is to provide experience with reading data from a file, writing data into a file, reversing data, sorting data, and evaluating the efficiency of the sorting algorithms. Note that, for all the paths of the files in this assignment, you should use the “relative” paths, rather than the “absolute” paths, in your Java program, because your directory structure in your own computer is often different from that of others (e.g., the graders) and using the “relative” paths will avoid this issue.

<ol>

 <li>Download the following file into the same directory as your Java program: <u>https://classes.cs.uoregon.edu/18S/cis212/examples/phonebook_test.txt</u></li>

</ol>

Write your Java program to read all the data from the above file into an ArrayList (which will be referred to as the “original” ArrayList hereafter) of the phonebook entries, where each entry consists of separate fields for the name and the phone number (e.g., a class with private String variables would be considered good). The file is a plain text file, where every line has the following format: “PhoneNumber LastName, FirstName”.

<ol start="2">

 <li>Implement a method that takes the original ArrayList of the phonebook entries and a String as inputs, and output all the phonebook entries which contain this input String in either the first name or the last name into another plain text file named “Output.txt” in the same directory as your Java program. Every line of this file should follow the same format as above.</li>

</ol>

For example, if the input String is “new”, then the following should be the content of your “Output.txt”:




If the input String is not contained by any name, then your “Output.txt” is an empty file.

<ol start="3">

 <li>Implement a recursive method (i.e., a method that invokes itself) which takes an ArrayList of phonebook entries as an argument and reverses the entries in this list. For example, assuming you read the list in the above picture into an ArrayList and invoke your method on this ArrayList, then after your method returns, this ArrayList should be as follows:</li>

</ol>







This is just a visualization. Here, unlike the previous two tasks of this assignment, you do not have to read data from a file and output data into a file.

<ol start="4">

 <li>Implement a method that takes the original ArrayList of the phonebook entries as an argument and returns a sorted copy of the list using Selection Sort to sort alphabetically by phonebook last name. Your implementation must not modify the original ArrayList.  You should implement your own sorting code here, and not use the Collections sort method.  Cite any source used in the comments of your code.</li>

 <li>Implement a method that takes the original ArrayList of the phonebook entries as an argument and returns a sorted copy of the list using Merge Sort to sort alphabetically by phonebook last name. Your implementation must not modify the original ArrayList.  Again, you should implement your own sorting code here, and not use the Collections sort method.  Cite any source used in the comments of your code.</li>

 <li>Implement a method that takes an ArrayList of the phonebook entries as an argument and returns true if the input list is already sorted alphabetically by phonebook last name (false otherwise). Your implementation must not modify the input list. Use this method to test your sorting implementations.</li>

 <li>Implement a method that invokes your own Selection Sort and Merge Sort codes, and report the elapsed <em>sorting</em> time in seconds, excluding the time of reading data from the file. Your output should look something like (but may not necessarily be):</li>

</ol>

Selection Sort: 27.094

Merge Sort: 0.433