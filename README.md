Download Link: https://assignmentchef.com/product/solved-comp-2710-project-4
<br>
<strong> </strong>




<strong><em><u>Goals:</u> </em></strong>

<ul>

 <li>To learn how to use linked data structures (Note: <strong>no array is allowed</strong>)</li>

 <li>To use strings</li>

 <li>To learn creating multiple versions via conditional compilation</li>

 <li>To design and implement functions</li>

 <li>To perform unit testing</li>

</ul>




In this homework assignment, you will write a simple trivia quiz game. Your program first allows players to create their trivia questions and answers. Multiple questions should be organized and managed using <strong><u>a linked data structured; no array is allowed in this homework assignment.</u></strong> Then, your program asks a question to the player, input the player’s answer, and check if the player’s answer matches the actual answer. If so, award the player the award points for that question. If the player enters the wrong answer your program should display the correct answer. When all questions have been asked, the total award points that the player has won should be displayed.




Please perform the following steps to finish this assignment.

<ul>

 <li><strong>Step 1: </strong>Create a TriviaNode <strong>structure </strong>that contains (1) information about a single trivia question and (2) a pointer pointing to other TriviaNode. This structure must contain a <strong>string</strong> for the question, a <strong>string </strong>for the answer to the question, an integer representing points the question is worth, and <strong>a pointer of the TriviaNode type. </strong>Please keep in mind that a harder question should be worth more points.</li>

</ul>







<ul>

 <li><strong>Step 2:</strong> Create a linked list of Trivia using the TriviaNode structure defined in step 1.</li>

</ul>







<ul>

 <li><strong>Step 3:</strong> Design and implement a function that initialize the Trivia linked list by hard-coding the following three trivia questions (including answers and award points). The o Trivia 1:</li>

</ul>

Question: How long was the shortest war on record? (Hint: how many minutes) Answer: 38

Award points: 100

<ul>

 <li>Trivia 2:

  <ul>

   <li>Question: What was Bank of America’s original name? (Hint: Bank of Italy or Bank of Germany) Answer: Bank of Italy</li>

  </ul></li>

</ul>

Award points: 50

<ul>

 <li>Trivia 3:

  <ul>

   <li>Question: What is the best-selling video game of all time? (Hint: Call of Duty or Wii Sports)?</li>

  </ul></li>

</ul>




Answer: Wii Sports

Award points: 20




<ul>

 <li><strong>Step 4: </strong>Design and implement a function to create and add a new TriviaNode into the linked list. You must use operator <strong>new </strong>to dynamic allocate memory to a new TriviaNode. Please remember to check that a new TriviaNode is successfully created.</li>

</ul>




<ul>

 <li><strong>Step 5:</strong> Design and implement a function that asks a question to the player, input the player’s answer, and check if the player’s answer matches the actual answer. If so, award the player the dollar amount for that question. If the player enters the wrong answer your program should display the correct answer.

  <ul>

   <li><strong>Input:</strong> a linked list of TriviaNode, the number of trivia to be asked in the list o <strong>Output:</strong> void or int – 0 indicates success and 1 indicates failure.</li>

  </ul></li>

</ul>




<ul>

 <li><strong>Step 6: </strong>Write a test driver to perform unit testing for the function implemented in step 5. Assume there are three trivia in your created list, you must cover at least the following cases: (see <strong> 1</strong> on page 3 for the sample user interface.) o Case 1: ask 0 question

  <ul>

   <li>Case 2: ask 1 question (i.e., the first one) from the list</li>

  </ul></li>

</ul>

Correct answer

Wrong answer

<ul>

 <li>Case 3: ask 3 questions (i.e., all the questions) from the list.</li>

</ul>

Correct answer

Wrong answer

<ul>

 <li>Case 4: ask 5 questions that exceed the number of available trivia in the linked list (i.e., the index of the trivia is larger than the size of the linked list).</li>

</ul>




<ul>

 <li><strong>Step 7:</strong> Write the main function that performs the following: (see <strong> 2</strong> on page 4 for the sample user interface)  o Create hard-code trivia quizzes (i.e., questions/answers/awards) (Note: just call  the function implemented in step 3).

  <ul>

   <li>Create more than 1 trivia quiz from a keyboard (Note: just call the function implemented in step 4).</li>

   <li>Write a for loop; in each iteration do the following:</li>

  </ul></li>

</ul>

asks a question to the player takes the player’s answer

compares the input answer with the actual answer

<ul>

 <li>if the player’s answer matches the actual answer, then award the player the corresponding award points for that question,</li>

 <li>else (i.e., the player enters the wrong answer) your program should display the correct answer.

  <ul>

   <li>When all questions have been asked, display the total award points the player has</li>

  </ul></li>

</ul>




<ul>

 <li><strong>Step 8: </strong>Create two versions using conditional compilation.</li>

</ul>




<ul>

 <li>Version 1: simply run the test driver implemented in step 6.</li>

 <li>Version 2: a regular version run the main function implemented in step 7.</li>

</ul>

Note: this version should not include the test driver.

You must provide the following user interface for the <strong>debug version</strong>. In this version, your  program must run the test driver you build in step 6.




<table width="642">

 <tbody>

  <tr>

   <td width="642">***This is a debugging version ***Unit Test Case 1: Ask no question. The program should give a warning message.  Warning – the number of trivia to be asked must equal to or be larger than 1.  Case 1 Passed Unit Test Case 2.1: Ask 1 question in the linked list. The tester enters an incorrect answer.Question: How long was the shortest war on record?Answer: 85Your answer is wrong. The correct answer is 38Your total points 0 Case 2.1 passed Unit Test Case 2.2: Ask 1 question in the linked list. The tester enters a correct answer.Question: How long was the shortest war on record?Answer: 38Your answer is correct! You receive 100 points.Your total points: 100 Case 2.2 passed Unit Test Case 3: Ask all the questions of the last trivia in the linked list. Question: How long was the shortest war on record?Answer: 38Your answer is correct! You receive 100 points. Your total points: 100 Question: What was Bank of America’s original name? (Hint: Bank of Italy or Bank of Germany)?Answer: Bank of GermanyYour answer is wrong. The correct answer is Bank of Italy.Your total points 100 show question here Add your answer here . . .Case 3 passed Unit Test Case 4: Ask 5 questions in the linked list. Warning – There is only 3 trivia in the list.Case 4 passed *** End of the Debugging Version ***</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>Fig. 1: Sample user interface for the debug version </strong>







You must provide the following user interface for the <strong>production version</strong>. The user input is depicted as <strong>Bold, </strong>but you do not need to display user input in bold. Please replace “Li” with your name. In this version, your program must run the test driver you build in step 6.

<table width="623">

 <tbody>

  <tr>

   <td width="623">*** Welcome to <strong>Li’s </strong>trivia quiz game ***Enter a question: enter your first question here.Enter an answer: enter your first answer here.Enter award points: enter your first award points here.Continue? (Yes/No): <strong>Yes</strong>Enter a question: enter your second question here.Enter an answer: enter your second answer here.Enter award points: enter your second award points here. Continue? (Yes/No): <strong>No</strong>Question: How long was the shortest war on record? (Hint: how many minutes) Answer: <strong>38</strong>Your answer is correct. You receive 100 points. Your total points: 100Question: What was Bank of America’s original name? (Hint: Bank of Italy orBank of Germany)?Answer: <strong>Bank of Germany</strong>Your answer is wrong. The correct answer is: Bank of Italy Your Total points: 100Question: What is the best-selling video game of all time? (Hint: Call of Duty or Wii Sports)?Answer: <strong>Wii Sports</strong>Your answer is correct. You receive 20 points. Your total points: 120…Display more questions/answers and information here……*** Thank you for playing the trivia quiz game. Goodbye! ***</td>

  </tr>

 </tbody>

</table>

<strong>Fig. 2: Sample user interface for the production version </strong>




<strong><em><u>How to Create Two Versions?</u> </em></strong>

You can use the preprocessor directive <strong>#ifdef</strong> to create and maintain two versions (i.e., a  debugging version and a product version) in your program. If you have the following code:




<ol>

 <li>#define UNIT_TESTING</li>

 <li>#ifdef UNIT_TESTING</li>

 <li>add your unit testing code here</li>

 <li>#else</li>

 <li>add your code for the product version here</li>

 <li>#endif</li>

</ol>




in your program, the code that is compiled depends on whether a preprocessor macro by that  name is defined or not. For example, if the UNIT_TESTING has been defined, i.e., line is enabled,  then line 3 ‘’ add your unit testing code here” is compiled and line 5 ‘’add your code for the product version here” is ignored. If the macro is not defined, i.e.,

line 1 is disabled, then line 5 ” add your code for the product version here” is compiled and line 3 “add your unit testing code here” is ignored.




These macros look a lot like if statements, but macros behave completely differently. More specifically, an <strong>if</strong> statement decides which statements of your program must be executed at run time, while a <strong>#ifdef</strong> controls which lines of code in your program are actually compiled.




<strong><em><u>Unit Testing:</u> </em></strong>

Unit testing is a way of determining if an individual function or class works as expected. You need to isolate a single function or class and test only that function or class. For each function in this homework, you need to check <u>normal cases and boundary cases.</u>




Examples for tested values:

<ul>

 <li>String – empty string, medium length, very long – Array – empty array, first element, last element</li>

 <li>Integer – zero, mid-value, high-value</li>

</ul>




You must implement a unit test driver for each function implemented in your program. You may  need to use assert() to develop your unit test drivers if tested results are predictable.




<strong><em><u>Integration Testing:</u> </em></strong>

Integration testing (a.k.a., Integration and Testing) is the phase in software testing in which individual software modules are combined and tested as a group. You may use the sample user interface illustrated in Fig. 2 on page 4 to perform an integration testing for your program.




<strong><em><u>Requirements:</u> </em></strong>

1.(2.5 points) Use comments to provide a heading at the top of your code containing your name, Auburn UserID, filename, and how to compile your code. Also describe any help or sources that you used (as per the syllabus).

2.(2.5 points) Your source code file should be named as “project4_lastname_userID.cpp”, e.g., project4_Liu_tzl0031.cpp.

3.(12.5 points) Your program must use structures and a linked list. (see steps 1-2)

4.(5 points) Your program must use string rather than char array. (see steps 1-2)

5.(5 points) A function that creates 3 hard-coding trivia quizzes. (see step 3)

6.(10 points) A function that creates new quiz from a keyboard. (see step 4)

7.(15 points) A function that asks a question and checks a player’s answer. (see step 5) 8.(15 points) Write a test driver for function implemented in step 5.

9.(10 points) Correctly implement the main function. (step 7)

<ol start="10">

 <li>(10 points) Create two versions using conditional compilation.</li>

 <li>(5 points) You must reduce number of global variables and data.</li>

 <li>(5 points) Usability of your program (e.g., user interface).</li>

 <li>(2.5 points) Readability of your source code.</li>

</ol>

<strong>Note</strong>: You will lose <strong>at least 40 points </strong>if there are compilation errors or warning messages when the TA compiles your source code. You will <strong>lose points</strong> if you: do not use the specific program file name, or do not have a comment, or don’t have a commend block on program you hand in.




<strong><em><u>Programming Environment:</u> </em></strong>

Write a short program in C++. Compile and run it using AU server (no matter what kind of editor you use, please make sure your code could run on AU server. The only test bed we accept is the AU server).





