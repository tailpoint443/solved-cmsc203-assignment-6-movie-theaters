Download Link: https://assignmentchef.com/product/solved-cmsc203-assignment-6-movie-theaters
<br>
In 1907 you could watch a film at a Nickelodeon theater for five cents. In fact, that’s why it’s called a “Nickel”odeon. During the Depression or the 1920s, movies cost about 27 cents. During the swinging ’60s, it cost a little less than $1 to catch a flick. The cost was about $4 to go during the 80’s and now you’re laying down a “10-spot” to watch a show.




Here’s some interesting facts about movie theaters:

<ul>

 <li>The first air-conditionedmovie theater was built way back in 1922,</li>

 <li>The first cup holders didn’t make it into cinemas until AMC Theatersintroduced them in 1981.</li>

 <li>The first shopping mall multiplex was built in 1963. It had two screens and sat 700 people.</li>

 <li>New Jersey was home to the very first drive-in theater, which was built in 1933. The drive-in theaterpeaked in popularity in the ’50s and ’60s but there are now less than 1000 of them left in North America.</li>

</ul>

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Description</strong></td>

  </tr>

 </tbody>

</table>













MOVIE TICKET MANGER




The XYZ Theater has four types of tickets Adult, Child, Employees, MoviePass. The price of the tickets are determined as follows:




Before 6pm     6pm and after  IMAX             3D                   Tax

Adult               $10.50             $13.50             +$3.00             +$2.50             +9.6%

Child               $5.75               $10.75             +$2.00             +$1.50             +9.6%

A CHILD can only attend G or PG movies




Employee – The first two movies are free and all additional movies are half of the pre-tax Adult price + 9.6% tax.




MoviePass – The first movie is $9.99 (includes tax) and all additional movies are free if:

<ol>

 <li>Attend only one movie per day</li>

 <li>Movie cannot have been seen before</li>

 <li>Movie cannot be IMAX or 3D.</li>

</ol>

If any of the 3 rules have not been met, they will be charged at the Adult price.







The Management of the XYZ Theater also wants to print reports of the following:

<ol>

 <li>All tickets</li>

 <li>3D tickets</li>

 <li>MoviePass tickets</li>

 <li>Monthly Sales Report</li>

</ol>




Create an application that calculates ticket prices and prints out reports needed by the management.

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Concepts tested by this assignment</strong></td>

  </tr>

 </tbody>

</table>













<ul>

 <li>Reading from a file</li>

 <li>ArrayList&lt;&gt;

  <ul>

   <li>Searching an Arraylist</li>

   <li>Sorting an Arraylist</li>

  </ul></li>

 <li>Enumeration</li>

 <li>Inheritance</li>

 <li>Interface</li>

 <li>Polymorphism

  <ul>

   <li>Abstract classes</li>

   <li>Overriding methods</li>

   <li>super()</li>

  </ul></li>

</ul>

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Classes</strong></td>

  </tr>

 </tbody>

</table>










<strong> </strong>




<strong>Data Element – Ticket</strong>

Create an abstract class called <strong>Ticket</strong> with:

<ul>

 <li>two abstract methods called <strong>calculateTicketPrice</strong> which returns a double and getId() which returns an int.</li>

 <li>instance variables (one of them is an object of the enumerated type Format) which are common to all the subclasses of Ticket</li>

 <li>toString method, getters and setters and at least 2 constructors, one of the constructors must be the default (no-arg) constructor.</li>

</ul>

<strong> </strong>

<strong>Data Element – subclasses of Ticket</strong>

Create the following classes for the 4 types of tickets: Adult, Child, Employee, MoviePass.

<ul>

 <li>may contain additional instance variables appropriate for the type of ticket. They will</li>

 <li>extend from Ticket and define the calculateTicketPrice and getId methods. The Adult and Child classes do not require an id, so getId will return a -1. There should be</li>

 <li>getters and setters for the instance variables, and any other methods that are needed for your design. The</li>

 <li>toString method and constructors for these classes will use the super reference to take advantage of the Ticket constructor and toString methods.</li>

 <li>Use finals to represent constants.</li>

</ul>

<strong> </strong>

<strong> </strong>

<strong> </strong>

<strong>Enumerated Type – Format</strong>

Create an enumerated type called Format.  The valid values will be IMAX and THREE_D and NONE.  (You are not allowed to start enumerated variables with a numeric, so 3D was not an option)

<strong> </strong>

<strong>Data Structure</strong>

<ul>

 <li>You will be using an Arraylist within your Data Manager to hold the ticket objects.</li>

</ul>

<strong> </strong>

<strong>Data Manager – MovieTicketManager</strong>

Create a MovieTicketManager class that implements the MovieTicketInterface.  It will contain:

<ul>

 <li>arraylist which holds references to Ticket objects (Adult, Child, Employee and MoviePass all inherit from Ticket).</li>

 <li>methods to add a ticket, calculate the total sales for the month, retrieve the 3D movie tickets, retrieve the MoviePass tickets, retrieve all tickets, and any other methods needed for your design.</li>

 <li>readFile method reads from a file and add tickets to the arrayList of Tickets</li>

 <li>toString method will polymorphically call the toString method for each ticket stored in the arraylist.</li>

 <li>monthlySalesReport method that returns a string with the entire report.</li>

 <li>suggest two private methods – sortById and sortByDay that will sort the arraylist of Ticket objects either by Id or by Day.</li>

 <li>Follow the Javadoc given you. Private members of the Javadoc are suggestions and are not required.</li>

</ul>

<strong>GUI Driver</strong>

<ul>

 <li>Create a GUI Driver class/classes. When the GUI is launched, tickets are added by reading from a file, or manually entered. Use the FileChooser dialog box to select the input file name. The fields in the file are separated by colons (:). You can assume all information in the file is correct.  The GUI will use an instance of the MoveTicketManager class.</li>

 <li>The user will have the ability to add additional employees through the keyboard. The labels and textfields will change depending on the type of movie patron that is selected to be added.</li>

 <li>Display a report of all movie tickets, 3D tickets and MoviePass tickets. All movie tickets and 3D ticket reports will be in order by date. MoviePass tickets reports are in numeric order by the moviepass id.</li>

 <li>Data Validation: If a CHILD ticket is being purchased, it can only be a G or PG movie rating. The time must be between 8 and 23 inclusively. The day must be between 1 and 31 inclusively.</li>

 <li>Note: your GUI need not display an icon.</li>

</ul>

<strong> </strong>

<strong>External Documentation</strong>

<ul>

 <li>Create Javadoc for all classes that you have created. Upload your entire doc folder.</li>

 <li>Provide a UML diagram with all classes and their relationships.</li>

</ul>

<strong> </strong>

<strong>Testing</strong>

<ul>

 <li>Ensure that the JUnit tests in MovieTicketManagerTest.java succeed.</li>

 <li>Implement the MovieTicketManagerTestSTUDENT test methods.</li>

 <li>Create a Junit test for your Adult and MoviePass classes.</li>

</ul>




<table width="100%">

 <tbody>

  <tr>

   <td><strong>Assignment Details</strong></td>

  </tr>

 </tbody>

</table>

The minimum information stored for each ticket:

<ul>

 <li>Movie name</li>

 <li>Rating</li>

 <li>Day</li>

 <li>Time</li>

 <li>ID (only needed for Employees and MoviePass members)</li>

 <li>Price of ticket</li>

</ul>







Reports needed by the Management:

<ul>

 <li>Print All Tickets (in order by date)</li>

 <li>Print 3D Tickets (in order by date)</li>

 <li>Print MoviePass Tickets (in order by MoviePass Id)</li>

 <li>Monthly Sales Report. Displays the total sales and number of each type of ticket sold that month. Also displays the total of all tickets sold that month</li>

</ul>

Use Alert boxes to display the reports.

<strong><u> </u></strong>

For simplicity sake, we will only be managing tickets for one month at a time. The day will be represented as an int (1-31)




For simplicity sake, movies start at the top of the hour and will be represented as an int in military format. The earliest movie will begin at 8 am (8) and the latest movie will begin at 11pm (23)

Movie ratings will be a string: G, PG, PG13, R, or NR.

INPUT FILES:

Input files that can be read from this application have values that are separated by a “:”.




SORTING:

Here is a simple Insertion Sort that works for arrays of ints:

<ol>

 <li>int temp;</li>

 <li>   for (int i = 1; i &lt; array.length; i++) {</li>

 <li>    for (int j = i; j &gt; 0; j–) {</li>

 <li>     if (array[j] &lt; array [j – 1]) {</li>

 <li>      temp = array[j];</li>

 <li>      array[j] = array[j – 1];</li>

 <li>      array[j – 1] = temp;</li>

 <li>     }</li>

 <li>    }</li>

</ol>

Convert this to work for an ArrayList of Ticket objects for your sortById and sortByDay methods.

When you sort by Day, don’t worry about ordering at a second level (such as time).

EMPLOYEE-45678 IMAX Movie: Book Club Rating: PG13 Day:1 Time: 19 Price: $0.00

MOVIEPASS-55555 IMAX Movie: Deadpool Rating: NR Day:1 Time: 23 Price: $14,80

Or:

MOVIEPASS-55555 IMAX Movie: Deadpool Rating: NR Day:1 Time: 23 Price: $14,80

EMPLOYEE-45678 IMAX Movie: Book Club Rating: PG13 Day:1 Time: 19 Price: $0.00

The JUnit test would consider both of these to be correct.




When you order by Id, don’t worry about ordering at a second level (such as day)




GUI:

Labels and Textfields will change depending on the type of ticket selected:




Print the Ticket Price in RED to make it easy to find:

<strong><u> </u></strong>

BUTTONS:

When the Purchase Ticket button is selected:

<ol>

 <li>Information will be gathered from the textfields and radiobuttons

  <ol>

   <li>data validation of day, time and CHILD ticket</li>

  </ol></li>

 <li>addTicket(…)</li>

 <li>Display the price of the ticket</li>

</ol>

When the Read File button is selected:

<ol>

 <li>User selects file with FileChoose</li>

 <li>readFile(..)</li>

 <li>Display the Monthly Total Sales</li>

</ol>










<table width="100%">

 <tbody>

  <tr>

   <td><strong>Examples</strong></td>

  </tr>

 </tbody>

</table>

<strong>Based on the following input file:</strong>

<strong><u> </u></strong>

<strong>Result of Print All Tickets: (in order by Day)</strong>

<strong><u> </u></strong>

<strong>Result of Print 3D Tickets:</strong>

<strong>Result of Print MoviePass Tickets:</strong>

<strong><u> </u></strong>

<strong>Result of Monthly Sales Report:</strong>

<strong><u> </u></strong>

<strong>Error Message – CHILD attempting to purchase a PG13 ticket.</strong>

<strong><u> </u></strong>

<strong>Error message – Time not valid</strong>

<strong><u> </u></strong>

<strong>Error Message – Day not valid</strong>

<strong><u> </u></strong>

<strong><u> </u></strong>

<table width="100%">

 <tbody>

  <tr>

   <td><strong>Deliverables</strong></td>

  </tr>

 </tbody>

</table>

<strong><u>Deliverables / Submissions</u>: </strong>

Design: UML class diagram with pseudo-code for key methods

Implementation: Submit a compressed file containing the follow (see below):  The Java application (it must compile and run correctly); Javadoc files in a directory; a write-up as specified below.  Be sure to review the provided project rubric to understand project expectations.  The write-up will include:

<ul>

 <li>UML diagram – latest version</li>

</ul>

<ul>

 <li>Any assumptions that you are making for this project</li>

 <li>In three or more paragraphs, highlights of your learning experience</li>

</ul>




<strong><u>Deliverable format</u>:</strong> The above deliverables will be packaged as follows. Two compressed files in the following formats:

<ul>

 <li>zip, a compressed file in the zip format, with the following:

  <ul>

   <li>Write up (Word document) – reflection paragraphs</li>

   <li>UML Diagram – latest version (Word or jpg document)</li>

   <li>doc (directory) – Javadoc</li>

  </ul></li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li>File1.html (example)</li>

       <li>File2.html (example)</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>

<ul>

 <li>src (directory) – Java and JUnit tests files</li>

</ul>

<ul>

 <li style="list-style-type: none;">

  <ul>

   <li style="list-style-type: none;">

    <ul>

     <li style="list-style-type: none;">

      <ul>

       <li>File1.java (example)</li>

       <li>File2.java (example)</li>

       <li>Filetest.java (example)</li>

      </ul></li>

    </ul></li>

  </ul></li>

</ul>

<ul>

 <li>zip, a compressed file containing one or more Java files:

  <ul>

   <li>java (example)</li>

   <li>java (example)</li>

   <li>java (example)</li>

   <li>This folder should contain Java source files only</li>

  </ul></li>

</ul>








