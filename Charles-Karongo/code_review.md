Project 3: Code Review and Static Analysis Summary
Charles Karongo CSCI-375 Software Engineering

## Overview

For Project 3 in software engineering, I worked on improving my Boggle solver through a full development and review cycle using GitHub, static analysis, unit testing, and a code review from our teaching assistant, Howard Prioleau. At the start, I actually struggled quite a bit with making Git commits and managing the branch workflow, but after working through the errors and figuring out what I was doing wrong, I finally got the hang of it and successfully added my code to the branch along with the rest of my classmates. The core of my project is a Boggle solver that uses depth-first search, recursive backtracking, and a prefix-checking trie to efficiently find all valid words on a grid while checking all eight neighboring directions and handling multi-letter tiles like Qu and St.

#Feedback I Gave To My Partner
Since I didn't review a student's code and was instead reviewed directly by TA Howard Prioleau, his feedback served as my primary evaluation for the project. He noted that my implementation made excellent use of dynamic programming and DFS, praised the solid code coverage across my unit tests, and suggested that I add a dedicated test suite specifically for Qu and St tiles to make the validation even more robust.

#Improvements I Implemented
Following Howard's review, I added the suggested multi-letter tile test suite for Qu and St, added clear docstrings and comments to help explain the search logic, and cleaned up my code's formatting to meet PEP 8 standards by fixing indentation, operator spacing, and long lines. I made sure these updates kept the underlying solver logic completely intact while improving readability and structure.

#Static Analysis Results
I ran pycodestyle on my updated code to catch any formatting or style issues, and it flagged minor things like spacing errors and trailing whitespaces. I fixed each one until the linter came back completely clean with zero errors, ensuring the code met all standard Python style guidelines.

#Regression Testing
After finishing the cleanup and adding the new test suite, I ran the full regression test suite in Codio to make sure nothing was broken by my edits. All the unit tests passed successfully across standard boards, edge cases, and the new tile tests, confirming the solver's correctness.

#Verification
I double-checked my local repository and test files to ensure the correct test suite was running and that my code was properly committed to the branch without any leftover temporary files or placeholder tests.

#Reflection
Reflecting on this assignment, the whole process really showed me how important it is to write clean, maintainable code rather than just code that happens to pass the tests. Getting past my initial Git frustrations and going through the review, linting, and testing steps gave me a much better feel for how software teams actually collaborate and build robust projects together.
