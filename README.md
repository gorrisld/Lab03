# Lab03

## Objective:
The objective of this Lab is to understand memory management approaches and implications those approaches.

This game implementation is trying to avoid the copy constructor being called on the Card class, as that could be akin to cheating.   In industry it could be that to create a new instance of a class is expensive, and the copy constructor is also expensive as well.

# Task

## Task 0: Evaluate initial starter implementation, to decide which two implementation to choose from.  You will be required to implement the RAII and std::move approach, but you also get to pick between dumb pointers or smart pointers.

YOu will be doing RAII and std::move, and then either dumb pointers or smart pointers.   

Compare and contrast the approaches towards managing the memory.

Run the code in the debugger to be able to help explain the difference if needed.

* Explain your choice for the project
*	Explain the difference between the copy and move constructor. (https://www.geeksforgeeks.org/move-constructors-in-c-with-examples/)
*	Explain why the unintentional calling of the copy constructor is bad (see the CallGameWithCheating in main.cpp)
*	Compare and contrast the destructors for the classes and approaches.  Which approach feels the one less prone to bugs?


## Task 1:  Consider how to Implement a card game called 13 using chosen implementations.

This will mean you need to modify the CMakeLists.txt file.  

The rules are:
1. Each Player starts with 5 cards in their hand
2. Player one plays first. When it is you turn a player can:
    a. start their win stack with a one/ace
    b. discard a card
    c. add to their win stack with the next highest number
    d. draw a card
3. A player's turn ends when they draw a card. A player can only have no more than 5 cards at any given time, and must have 5 cards when their turn is over.
4. The game ends when a player completes their stack with all cards (ace-king or 1-13).

## Task 2  Create a Unit Test library to test the classes for the two implementations.
Write and have pass at least 3 tests per class (3 classes, so so min of 9 UnitTests per each implementation).  These tests do not have to be super complicated, but this is where you want to think about your corner cases.

Complete this before moving on to task 3.
 
## Task 3 Now provide implementation for the approachs you chose in Task 0 and implement the card game 13.
Show screen shots of you two games with an initial hand, and a screen shot of the game ending with a player winning.  Do this for both implementations.


# Lab Submission
1.	Write a PDF that has the screenshots or written sections asked for in the Tasks (if applicable)
3.	Include all source code from all tasks, input and output files (if any), and any special instructions to compile and run those programs.
4.	Package all source files in a single tar and submit the file to canvas.  (so submit two files a tar files and pdf file)

# Lab Grading
1.	60% - code has been correctly implemented and meets all requirements.
1.	40% - Code style, Participation Rubric, and Information requested in PDF 

If program fails to compile, 0% will be given for that Task.
