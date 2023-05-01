Download Link: https://assignmentchef.com/product/solved-assignment-5-object-relationship-and-file-io
<br>
<h3 id="sites-page-title-header" align="left"></h3>

5/5 - (1 vote)

<table class="sites-layout-name-one-column sites-layout-hbox" style="height: 5250px;" width="1009" cellspacing="0">

 <tbody>

  <tr>

   <td class="sites-layout-tile sites-tile-name-content-1"></td>

  </tr>

 </tbody>

</table>

<p dir="ltr">Write a program to perform statistical analysis of scores for a class of students.The class may have up to 40 students.There are five quizzes during the term. Each student is identified by a four-digit student ID number.

<p dir="ltr">The program is to print the student scores and calculate and print the statistics for each quiz. The output is in the same order as the input; no sorting is needed. The input is to be read from a text file. The output from the program should be similar to the following:

<p dir="ltr">Here is some sample data (not to be used) for calculations:

<p dir="ltr">Stud Q1 Q2 Q3 Q4 Q5

<p dir="ltr">1234 78 83 87 91 86

<p dir="ltr">2134 67 77 84 82 79

<p dir="ltr">1852 77 89 93 87 71

<p dir="ltr">High Score 78 89 93 91 86

<p dir="ltr">Low Score 67 77 84 82 71

<p dir="ltr">Average     73.4    83.0    88.2     86.6    78.6

<p dir="ltr">The program should print the lowest and highest scores for each quiz.

<h1 dir="ltr"><a name="TOC-Plan-Of-Attack"></a>Plan Of Attack</h1>

<p dir="ltr">Learning Objectives

<p dir="ltr">You will apply the following topics in this assignment:

<ul>

 <li dir="ltr"><p dir="ltr">File Input operations.</li>

 <li dir="ltr"><p dir="ltr">Working and populating an array of objects.</li>

 <li dir="ltr"><p dir="ltr">Wrapper Classes.</li>

 <li dir="ltr"><p dir="ltr">Object Oriented Design and Programming.</li>

</ul>

<h2 dir="ltr"><a name="TOC-Understanding-requirements"></a>Understanding requirements</h2>

<p dir="ltr">Here is a copy of actual data to be used for input.

<p dir="ltr">Stud Qu1 Qu2 Qu3 Qu4 Qu5

<p dir="ltr">1234 052 007 100 078 034

<p dir="ltr">2134 090 036 090 077 030

<p dir="ltr">3124 100 045 020 090 070

<p dir="ltr">4532 011 017 081 032 077

<p dir="ltr">5678 020 012 045 078 034

<p dir="ltr">6134 034 080 055 078 045

<p dir="ltr">7874 060 100 056 078 078

<p dir="ltr">8026 070 010 066 078 056

<p dir="ltr">9893 034 009 077 078 020

<p dir="ltr">1947 045 040 088 078 055

<p dir="ltr">2877 055 050 099 078 080

<p dir="ltr">3189 022 070 100 078 077

<p dir="ltr">4602 089 050 091 078 060

<p dir="ltr">5405 011 011 000 078 010

<p dir="ltr">6999 000 098 089 078 020

<p dir="ltr">Essentially, you have to do the following:

<ul>

 <li dir="ltr"><p dir="ltr">Read Student data from a text file.</li>

 <li dir="ltr"><p dir="ltr">Compute High, Low and Average for each quiz.</li>

 <li dir="ltr"><p dir="ltr">Print the Student data and display statistical information like High/Low/Average..</li>

</ul>

<h2 dir="ltr"><a name="TOC-Design"></a>Design</h2>

<p dir="ltr">This program can be written in one class. But dividing the code into simple and modular classes based on functionality, is at the heart of Object Oriented Design.

<p dir="ltr">You must learn the concepts covered in the class and find a way to apply.

<p dir="ltr">Please make sure that you put each class in its own .java file.

<p dir="ltr">package lab2;

<p dir="ltr">class Student {

<p dir="ltr"> private int SID;

<p dir="ltr"> private int scores[] = new int[5];

<p dir="ltr"> //write public get and set methods for

<p dir="ltr"> //SID and scores

<p dir="ltr"> //add methods to print values of instance variables.

<p dir="ltr">}

<p dir="ltr">/************************************************************************************/

<p dir="ltr">package lab2;

<p dir="ltr">class Statistics

<p dir="ltr">{

<p dir="ltr"> int [] lowscores = new int [5];

<p dir="ltr"> int [] highscores = new int [5];

<p dir="ltr"> float [] avgscores = new float [5];

<p dir="ltr"> void findlow(Student [] a){

<p dir="ltr">/*This method will find the lowest score and store it in an   array names lowscores. */

<p dir="ltr"> }

<p dir="ltr">  void findhigh(Student [] a){

<p dir="ltr">/* This method will find the highest score and store it in an     array names highscores. */

<p dir="ltr"> }

<p dir="ltr"> void findavg(Student [] a){

<p dir="ltr">/* This method will find avg score for each quiz and store it in an array names avgscores. */

<p dir="ltr"> }

<p dir="ltr"> //add methods to print values of instance variables.

<p dir="ltr">}

<p dir="ltr">************************************************************************************/

<p dir="ltr">package lab2;

<p dir="ltr">class Util {

<p dir="ltr">static Student [] readFile(String filename, Student [] stu) {

<p dir="ltr">//Reads the file and builds student array.

<p dir="ltr">//Open the file using FileReader Object.

<p dir="ltr">//In a loop read a line using readLine method.

<p dir="ltr">//Tokenize each line using StringTokenizer Object

<p dir="ltr">//Each token is converted from String to Integer using parseInt method

<p dir="ltr">//Value is then saved in the right property of Student Object.

<p dir="ltr">}

<p dir="ltr">}

<p dir="ltr">************************************************************************************/

<p dir="ltr">//Putting it together in driver class:

<p dir="ltr">     public static void main(String [] args) {

<p dir="ltr">Student lab2 [] = new Student[40];

<p dir="ltr">//Populate the student array

<p dir="ltr">lab2 = Util.readFile(“filename.txt”, lab2)

<p dir="ltr">Statistics statlab2 = new Statistics();

<p dir="ltr">statlab2.findlow(lab2);

<p dir="ltr">//add calls to findhigh and find average

<p dir="ltr">//Print the data and statistics

<p dir="ltr">     }

<h2 dir="ltr"><a name="TOC-Topics-to-Learn"></a>Topics to Learn</h2>

<h3 dir="ltr"><a name="TOC-Working-with-Text-files"></a>Working with Text files</h3>

<p dir="ltr">//ReadSource.java — shows how to work with readLine and FileReader

<p dir="ltr">public class ReadSource {

<p dir="ltr">   public static void main(String[] arguments) {

<p dir="ltr">    try {

<p dir="ltr">FileReader file = new            FileReader(“ReadSource.java”);

<p dir="ltr">          BufferedReader buff = new

<p dir="ltr">               BufferedReader(file);

<p dir="ltr">           boolean eof = false;

<p dir="ltr">           while (!eof) {

<p dir="ltr">               String line = buff.readLine();

<p dir="ltr">               if (line == null)

<p dir="ltr">                  eof = true;

<p dir="ltr">               else

<p dir="ltr">                   System.out.println(line);

<p dir="ltr">           }

<p dir="ltr">           buff.close();

<p dir="ltr">       } catch (IOException e) {

<p dir="ltr">           System.out.println(“Error — ” + e.toString());

<p dir="ltr">       }

<p dir="ltr">   }

<p dir="ltr">}

<p dir="ltr">//How do you tokenize a String? You can use other ways of doing this, if you like.

<p dir="ltr">    StringTokenizer st = new StringTokenizer(“this is a test”);

<p dir="ltr">    while (st.hasMoreTokens()) {

<p dir="ltr">        System.out.println(st.nextToken());

<p dir="ltr">    }

<p dir="ltr">//How to convert a String to an Integer

<p dir="ltr">    int x = Integer.parseInt(String) ;

<h2 dir="ltr"><a name="TOC-Submitting-your-work"></a>Submitting your work</h2>

<p dir="ltr">Before submitting your work, please reflect on following points:

<ol>

 <li dir="ltr"><p dir="ltr">No errors, program always works correctly and meets the  specification(s) (2 points).</li>

 <li dir="ltr"><p dir="ltr">The code could be reused as a whole or each routine could be  reused (2 points).</li>

 <li dir="ltr"><p dir="ltr">Concepts of OOD are applied (7 points):

  <ol>

   <li dir="ltr"><p dir="ltr">Usage of OOP constructs, relationships, interface and abstract classes.</li>

   <li dir="ltr"><p dir="ltr">Code organized into functionally relevant packages – e.g. Util, Model etc. in  their own respective packages.</li>

   <li dir="ltr"><p dir="ltr">File IO API applied.</li>

  </ol></li>

 <li dir="ltr"><p dir="ltr">Need to follow Java coding conventions (2 points).</li>

 <li dir="ltr"><p dir="ltr">Code Readability (as suggested in class) (2 points).</li>

 <li dir="ltr"><p dir="ltr">Adequately tested (unique test cases, covering boundary conditions) (2 points).</li>

 <li dir="ltr"><p dir="ltr">Class diagram is provided (UML usage is not required) (3 points).</li>