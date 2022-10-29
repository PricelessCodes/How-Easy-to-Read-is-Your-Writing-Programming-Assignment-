# How-Easy-to-Read-is-Your-Writing-Programming-Assignment-
Data Structures and Performance University of California San Diego Course from Coursera.

Programming Assignment: How Easy to Read is Your Writing?

Getting Set Up
1. (If not already done) Download and set up the starter code

Before you begin this programming assignment, you need to download and set up the starter code. You should have already followed the instructions for setting up Java and Eclipse. Make sure you have the most recent version of the starter code by checking the date the starter code was last updated.  You are welcome to use any IDE of your choice, but we provide the starter code as an Eclipse project, so you'll probably find it easiest to work in Eclipse.

Make sure you've followed the setup instructions even if you've previously worked with Eclipse, and even if you took the first course in our series, because you'll need to make sure you have some additional pieces installed and set up (e.g. At least Java 1.8, JUnit).

2. Verify that the front-end runs

Make sure the project you downloaded and set up for this course is open in eclipse. 

As you saw in Mia's demo video, all of the functionality you will implement in this course will be integrated into a text editor application.  You can already run this application, but it won't do much.

Run the text editor by running the MainApp class inside the application package.  You can do this by expanding the application package in the package explorer and then selecting the MainApp.java file and running it.

![image](https://user-images.githubusercontent.com/66659379/198825433-16865ef0-80eb-4783-9913-8e959d5f85e1.png)

You will see a text editor window open.  You can type in the text window and load text using the "Load" button.  None of the other buttons work yet (you can click them, but they don't do anything). But they will soon...

3. Orient yourself to the starter code

Open the starter code for this assignment by expanding the document package in the Package Explorer window.  There you will see several files, but the two that are relevant to this assignment are Document.java and BasicDocument.java.  Open these by double-clicking on them.  

Notice that Document is an abstract class.  BasicDocument will implement the abstract methods in the 
Document class using the guidelines below described in the parts below.  

Assignment Details
This assignment is divided into two parts.  You will submit a separate file for each part, as described below.

Part 1: Implement the missing methods in BasicDocument.java
1. Implement getNumSentences, getNumWords and getNumSyllables following the comments about how they are supposed to work that you will find in your starter code (the version uploaded June 22, 2016 or later has the most detailed comments).  You'll probably also want to implement countSyllables(String) in Document.java, to be called in getNumSyllables.

You must follow the definitions of what constitutes a syllable, word and sentence given in the documentation for each function exactly to pass the graders.

We have provided you will several test cases in main as well as a helper method you can use to write your own tests.

2. Part 1 Bonus (purely optional, just for fun):  

Our REGEX are pretty naive.  For example, the word 7.5 causes real problems for our expressions as a “.” usually denotes the end of a sentence.  If you want to learn more about REGEX, you can improve upon our approach.  But if you want to do this, put it in a separate class (like ImprovedDocument) and make sure you don't use it to produce your grading output.

Part 2: Implement the getFleschScore method in Document.java

1. Fill in the method getFleschScore() in Document.java to calculate the Flesch Score for the text in the document.  You should use the following formula, and make calls to the getNumSyllables, getNumWords, and getNumSentences you just implemented.

![image](https://user-images.githubusercontent.com/66659379/198825503-b0450f99-652c-49b4-a603-82157034dfa9.png)

You should test your code by calculating the Flesch score by hand on some very basic documents and then calling your method from main to make sure it's giving the same output.  Or you can go ahead and run our grader before you submit, which you can find in the same package.
