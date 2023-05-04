Download Link: https://assignmentchef.com/product/solved-cse-231-computer-project-4
<br>
(Edit 2/6: output in this document now match tests on Mimir.)




This assignment focuses on the design, implementation and testing of a Python program to calculate and display the values of selected mathematical functions (see below).

In this assignment, you will practice with functions.

<h2>Assignment Background</h2>

<strong> </strong>

Many common mathematical functions can be expressed as the sum of a series of terms.  In some cases (such as the sum of the first N natural numbers), the function can be expressed as a finite series of terms.




In other cases, the expression contains an infinite number of terms.  For example, the tangent function can be expressed as the infinite series:










(GIF courtesy of Wikipedia)




<h2>Assignment Specifications</h2>

<strong> </strong>

You will develop a Python program which allows the user to select from a menu of options and which performs the requested calculations.  You must use at least the four functions specified below. You are encouraged to use more functions of your own design. Global variables are not allowed. That is, any variable names used within any function must be parameters or be created in the function. You are not allowed to use advanced data structures such as list, dictionaries, classes, etc. However, you are allowed to read ahead and use try-except.




<strong>sum_natural_squares (N) —</strong>à<strong> int:</strong>

<ol>

 <li>This function accepts as the user input (string) as numerical value and returns the sum of the <strong>squares</strong> of the first N natural numbers. If the user input is not a natural number (an integer &gt; 0), the function should return None. Note the string method .isdigit() is helpful.</li>

 <li>Parameters: N (string)</li>

 <li>Returns : int or None</li>

 <li>The function displays nothing.</li>

</ol>







<strong>approximate_pi () —</strong>à<strong> float:</strong>

<ol>

 <li>This function accepts no input and returns the approximate of Pi (p ). The number should be <strong>rounded</strong> to 10 decimal digits after the decimal point. The number is calculated as:</li>

</ol>

p=4*æçå¥ <u>(</u>-1<u>)</u><em>n </em>ö÷

ç<em>n</em>=0 2 1<em>n</em>+ ÷ø è

The program will expand the series until the <strong>absolute value</strong> of the next term in the series is less than 1.0e-7 (the specified epsilon); that term will <strong>not</strong> be included in the sum.

<ol>

 <li>Parameters: no parameters</li>

 <li>Returns : float</li>

 <li>The function displays nothing.</li>

</ol>




<strong>approximate_</strong> <strong>sin(x)—</strong>à<strong> float:</strong>

<ol>

 <li>This function accepts as input a numeric value X (measured in radians) and returns the approximate value of the sine of X. The number should be <strong>rounded</strong> to 10 decimal digits after the decimal point. The number is calculated as:</li>

</ol>




<h2>sin(<em>x</em>)=å<em>n</em>¥=0 (-(21<em>n</em>)<em>n</em>+<em>x</em>1 !2 1)<em>n</em>+</h2>

The program will expand the series until the <strong>absolute value</strong> of the next term in the series is less than 1.0e-7 (the specified epsilon); that term will <strong>not</strong> be included in the sum. The parameter is a string; if it isn’t in the correct format for a float, return None. c. Parameters: x (str)

<ol>

 <li>Returns : float or None</li>

 <li>The function displays nothing.</li>

</ol>




<strong>approximate_</strong> <strong>cos(x)—</strong>à<strong> float:</strong>

<ol>

 <li>This function accepts as input a numeric value X (measured in radians) and returns the approximate value of the cosine of X. The number should be <strong>rounded</strong> to 10 decimal digits after the decimal point. The number is calculated as:</li>

</ol>




cos(<em>x</em>)=å¥=0 (-(12 !)<em>n</em><em>n</em>)<em>x</em>2<em>n</em>

<em>n</em>

The program will expand the series until the <strong>absolute value</strong> of the next term in the series is less than 1.0e-7 (the specified epsilon); that term will <strong>not</strong> be included in the sum. The parameter is a string; if it isn’t in the correct format for a float, return None. b. Parameters: x (str)

<ol>

 <li>Returns : float or None</li>

 <li>The function displays nothing.</li>

</ol>




<strong>  main():  </strong>

<ol>

 <li>This function is used to interact with the user. It takes no input and returns nothing. Call the functions from here. The program should prompt the user to choose between 6 options (<u>capitalization does not matter</u>) until the user enters ‘X’:</li>

</ol>

‘A’  –  Display the value of the sum of squares of the first N natural numbers.

‘B’  –  Display the approximate value of Pi.

‘C’  –  Display the approximate value of the sine of X.

‘D’  –  Display the approximate value of the cosine of X.

‘M’ –  Display the menu of options.      ‘X’ –  Exit from the program.

<ol>

 <li>The program will repeatedly prompt the user to enter a letter (upper or lower case) which corresponds to one of the supported options. For example, the user will enter the letter A (or the letter a) to select Option A (display the value of the sum of the first N natural numbers).</li>

 <li>The program will display the menu of options once when execution begins, whenever the user selects Option M, and whenever the user selects an invalid menu option.</li>

 <li>If the user enters option A, the program will ask the user to enter a numeric value N. If N is a natural number, the program will calculate and display the value of the sum of squares of the first N natural numbers. Otherwise, the program will display an appropriate message.</li>

 <li>If the user enters option B, the program will calculate and display the approximate value of Pi. It will then display the corresponding value from the Python math module, as well as the absolute value of the difference between the calculated value and the math module value. The program should display 10 decimal digits after the decimal point for the approximate value. Use the appropriate string formatting.</li>

 <li>If the user enters option C, the program should ask the user to enter a numeric value X (measured in radians). The program will calculate and display the approximate value of the sine of X. It will then display the corresponding value from the Python math module, as well as the absolute value of the difference between the calculated value and the math module value. The program should display 10 decimal digits after the decimal point for the approximate value.  Use the appropriate string formatting.</li>

 <li>If the user enters option D, the program will ask the user to enter a numeric value X</li>

</ol>

(measured in radians).  The program will calculate and display the approximate value of the cosine of X. It will then display the corresponding value from the Python math module, as well as the absolute value of the difference between the calculated value and the math module value. The program should display 10 decimal digits after the decimal point for the approximate value.  Use the appropriate string formatting.

<ol>

 <li>If the user quits, the program should display a goodbye message.</li>

</ol>







<h3>Assignment Notes and Hints</h3>




<ol>

 <li>The coding standard for CSE 231 is posted on the course website:</li>

</ol>




<u>http://www.cse.msu.edu/~cse231/General/coding.standard.html</u>




Items 1-9 of the Coding Standard will be enforced for this project.




<ol start="2">

 <li>The program will produce reasonable and readable output, with appropriate labels for all values displayed.</li>

</ol>




<ol start="3">

 <li>You may assume that the user enters a string representing a numeric value when prompted for a number. However, you should not assume that the value is valid in that particular context.  For example, the user might enter 45.7 for Option A; that numeric value is not a natural number.</li>

</ol>




<ol start="4">

 <li>Be sure to prompt the user for the inputs in the correct order. And, your program cannot prompt the user for any supplementary inputs.</li>

</ol>




<ol start="5">

 <li>Several items from the math module might be useful for this project:</li>

</ol>




math.pi

math.fabs()  math.factorial()    math.sin()  math.cos()




<ol start="6">

 <li>The program will calculate the value for Option A using either a loop or an equation.</li>

</ol>




<ol start="7">

 <li>We provide a py program for you to start with.</li>

</ol>




<ol start="8">

 <li>You are not allowed to use advanced data structures such as list, dictionaries, classes, etc. However, you are allowed to read ahead and use try-except.</li>

</ol>




<ol start="9">

 <li>If you “hard code” answers, you will receive a grade of zero for the whole project. An example of hard coding is to simply print the approximate value of e rather than calculating it and then printing the calculated average.</li>

</ol>




<ol start="10">

 <li>There are multiple ways to check whether a string contains a float. One is to use the float_check function you developed in Lab 4.  That function doesn’t consider a float in the format such as 4e2, but that is fine for this project—we will assume that the user will not use that format for input.  However, the best way to check for a float is to use the try-except from Section 6.6.2 of the text.  You try to convert a value to a float and if a ValueError exception is raised you handle it, e.g. return None.  Feel free to read ahead and use the tryexcept statement in this project.</li>

</ol>




<ol start="11">

 <li>Good style defines a constant EPSILON = 1.0e-7</li>

</ol>




<strong> </strong>

<h3>Suggested Procedure</h3>

<strong> </strong>

<ul>

 <li><em>Solve the problem using pencil and paper first.</em> You cannot write a program until you have figured out how to solve the problem.  This first step can be done collaboratively with another student.  However, once the discussion turns to Python specifics and the subsequent writing of Python statements, you must work on your own.</li>

</ul>




<ul>

 <li>Cycle through the following steps to incrementally develop your program:</li>

</ul>




<ul>

 <li>Edit your program to add new capabilities.</li>

 <li>Run the program and fix any errors.</li>

 <li>Use the <strong>Mimir</strong> system to submit the current version of your program.</li>

</ul>




<ul>

 <li>Be sure to use the <strong>Mimir</strong> system to submit the final version of your program.</li>

</ul>




<ul>

 <li>Be sure to log out when you leave the room, if you’re working in a public lab.</li>

</ul>




<em>The last version of your solution is the program which will be graded by your TA. </em>

<em> </em>

<em>You should use the <strong>Mimir</strong> system to back up your partial solutions, especially if you are working close to the project deadline.  That is the easiest way to ensure that you won’t lose significant portions of your work if your machine fails or there are other last-minute problems. </em>




<strong> </strong>

<strong> </strong>

<strong> </strong>

<h3>Assignment Deliverable</h3>




The deliverable for this assignment is the following file:




proj04.py – the source code for your Python program




Be sure to use the specified file name and to submit it for grading via the <strong>Mimir</strong> <strong>system</strong> before the project deadline.







<strong>Test 1: </strong>







Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: n




Error:  unrecognized option [N]




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: M




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: X

Hope to see you again.




<strong> </strong>

<strong>Test 2: </strong>

<strong> </strong>

Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: n




Error:  unrecognized option [N]




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: M




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: X

Hope to see you again.

RJE-MacBook <strong>Admin </strong>% cat output2.txt




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: a




Enter N: 0




Error: N was not a valid natural number. [0]




Enter option: A




Enter N: 1.6




Error: N was not a valid natural number. [1.6]




Enter option: a




Enter N: 6




The sum:  91




Enter option: x

Hope to see you again.

<strong> </strong>

<strong>Test 3: </strong>

<strong> </strong>

Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: b




Approximation: 3.1415924536      Math module:   3.1415926536     difference:    0.0000000200




Enter option: C




Enter X: a




Error: X was not a valid float. [a]




Enter option: c




Enter X: 1.5




Approximation: 0.9974949557      Math module:   0.9974949866     difference:    0.0000000309




Enter option: C




Enter X: 0




Approximation: 0.0000000000      Math module:   0.0000000000     difference:    0.0000000000




Enter option: x

Hope to see you again.




<strong>Test 4: </strong>




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: d




Enter X: kl




Error: X was not a valid float. [kl]




Enter option: 0




Error:  unrecognized option [0]




Please choose one of the options below:

<ol>

 <li>Display the sum of squares of the first N natural numbers.</li>

 <li>Display the approximate value of Pi.</li>

 <li>Display the approximate value of the sine of X.</li>

 <li>Display the approximate value of the cosine of X.</li>

 <li>Display the menu of options.</li>

 <li>Exit from the program.</li>

</ol>




Enter option: D




Enter X: 0




Approximation: 1.0000000000      Math module:   1.0000000000     difference:    0.0000000000




Enter option: d




Enter X: 4




Approximation: -0.6536436057     Math module:   -0.6536436209    difference:    0.0000000152




Enter option: d




Enter X: 1.5




Approximation: 0.0707372050

Math module:   0.0707372017  difference:    0.0000000033




Enter option: x

Hope to see you again.

<strong> </strong>

<h3>Grading Rubric</h3>




Computer Project #04                           Scoring Summary

General Requirements:

( 4 pts) Coding Standard 1-9

(descriptive comments, function headers, mnemonic identifiers, format, etc…)




Implementation:

( 4 pts)  sum_natural_squares() function




( 5 pts)  approximate_pi() function




( 5 pts)  approximate_ sin() function




( 5 pts)  approximate_ cos() function




( 3 pts)  Test 1




( 4 pts)  Test 2




( 5 pts)  Test 3




( 5 pts)  Test 4










Note: hard coding an answer earns zero points for the whole project -10 points for not using main()