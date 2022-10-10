---
toc: true
layout: post
description: Planning our Program
categories: [week7, csp, ap]
image: 
title: Program Design and Development
---

# Program Basics
- Our program will be a notes site which allows users to store their notes for classes. 
- We plan to store the notes so a user can make specific folders for certain classes.
- Also, we want the user to access the notes, even after closing the site.

# Plan
Develop each aspect of code -> Run the code -> Optimize code -> Add to big project

How we could approach development:
1. Develop a way for users to input questions and answers
2. Develop a way for users to store the flashcards as a named set
3. Create a way for users to access cards.
4. Develop a way for users to place flashcard sets in a folder
5. Create a way for users to access cards.
6. Develop a login system.
7. Create example sets.

# Program Info
Program Purpose and Function
- The purpose of the program is to randomly generate questions based on a user’s notes of key terms/dates/ideas and definitions. The program will take the user’s notes and, based on it, select the key terms and output multiple quiz questions which will be displayed randomly. It will score the quiz and tell you what you got wrong and what you need to study on.

Data Abstraction
- The program will contain lists and dictionaries. Every key term will have a definition and these will be stored in a dictionary which will be stored in a list. Or they will be stored in a local database and we will use the objects in the database to create the quiz.

Managing Complexity
- The dictionaries and databases will manage the complexity of the program by organizing the data inputted by the user. It will also help calling back to create the quiz.

Procedural Abstraction
- A function will be created to call back to the data inputted by the user. The function will iterate over the dictionary/database and use the values in them as a parameter to make a quiz.

Algorithm Implementation
- Like stated before, the program will contain a function that uses iteration and sequencing to make a quiz based off the data inputted by the user that is saved in a database or dictionary.

Testing
- The function will be called each time the user inputs a note and each time the user generates a quiz. When the user inputs a note, the function is called and saves the note inside a dictionary or database. When the user presses the button that generates the quiz, the function is again called and iterates through the user’s notes to generate a quiz that is related to the key terms the user inputted.

# How it aligns with Standards
1. Instructions for input from one of the following: the user, a device, an online data system, a file
- Our project will take in user input and be able to save data for specific users.
2. Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the program’s purpose
- We will store question and answer sets in either lists or dictionaries.
3. At least one procedure that contributes to the program’s intended purpose, where you have defined: the procedure's name, the return type, one or more parameters
- We will be able to return question and answer sets and store them under a name.
4. An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure
- We will have to create a random selection algorithm for our
5. Calls to your student-developed procedure
- The program will feature unique student created procedure to call back to.
6. Instructions for output (tactile, audible, visual, or textual) based on input and program functionality
- The outputs could have correct and incorrect screen for the user. 