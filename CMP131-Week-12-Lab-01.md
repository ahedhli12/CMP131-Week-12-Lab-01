# CMP 131 – Python Programming


> **Required file location:** Keep every Python file directly in the repository root. Do not create a `src` folder.

## Week 12 – Lab 1: String Manipulation

**Total Points: 100**

## Learning Objectives

After completing this lab, students should be able to:

* Create and store a string in a variable.
* Accept string input from the user.
* Remove unnecessary spaces from a string.
* Determine the length of a string.
* Access individual characters using positive and negative indexes.
* Extract portions of a string using slicing.
* Convert a string to uppercase and lowercase.
* Replace part of a string with different content.
* Split a string into a list of words.
* Use a loop to process the words or characters in a string.
* Display string-processing results using clear labels.
* Organize a Python program using a `main()` function.
* Use comments to explain major program sections.

## Assignment Overview

Create a Python program that demonstrates several string-manipulation techniques.

The program will:

1. Ask the user to enter a sentence or phrase.
2. Store the entry in a string variable.
3. Remove unnecessary spaces from the beginning and end.
4. Display the first and last characters.
5. Display the length of the string.
6. Extract and display several substrings.
7. Convert the string to uppercase and lowercase.
8. Replace selected content in the string.
9. Split the string into individual words.
10. Use a loop to process either the words or the characters.

The instructor is not providing completed Python code or an exact output design. Students must design, write, and test their own programs.

## Required Python File

Create a Python file named:

`string_manipulation.py`

Include a comment header containing:

* Student name
* Course number
* Week number
* Lab number
* Assignment title
* Date

Example header structure:

```python
# Student Name:
# Course: CMP 131
# Week: 12
# Lab: 1
# Assignment: String Manipulation
# Date:
```

# Program Requirements

## Part 1: Display a Program Title

Display a descriptive title when the program begins.

Example:

```text
STRING MANIPULATION PROGRAM
```

Students may create their own title and output design.

## Part 2: Create the String Variable

Ask the user to enter a sentence or phrase.

Example prompt:

```text
Enter a sentence or phrase:
```

Store the user’s entry in a meaningful string variable.

The program must not continue with an empty string. If the user enters only spaces:

* Display an appropriate error message.
* Ask the user to enter the sentence again.
* Continue until the user provides valid text.

Keep the original string available so that it can be compared with the modified versions.

## Part 3: Remove Unnecessary Spaces

Use the `strip()` method to remove unnecessary spaces from the beginning and end of the user’s entry.

Store the result in a separate variable.

Display both:

* The original string
* The stripped string

Use clear labels so the user can see the effect of `strip()`.

For example:

```text
Original string: "  Python programming is fun!  "
Stripped string: "Python programming is fun!"
```

The quotation marks in the output are optional, but they may help show where leading or trailing spaces were removed.

Use the stripped string for the remaining operations.

## Part 4: Display Basic String Information

Use string indexing and the `len()` function to display:

* The first character
* The last character
* The total number of characters

The first character should be accessed using index `0`.

The last character should be accessed using negative indexing.

Spaces and punctuation inside the string count as characters when calculating the length.

Display each result with a clear label.

Example structure:

```text
First character: P
Last character: !
Number of characters: 26
```

Do not manually enter the characters or length. The values must be obtained from the string.

## Part 5: Slice the String

Use string slicing to extract and display the following substrings:

* The first five characters
* The last five characters
* The characters beginning at index `2` and ending before index `7`

Display each slice using a descriptive label.

Example structure:

```text
First five characters:
Last five characters:
Characters from index 2 through 6:
```

Python slicing does not cause an error if the string contains fewer than five or seven characters. The program should still display the available characters.

Do not manually copy characters from the string. Each substring must be created using a slicing expression.

## Part 6: Change the Letter Case

Use the following string methods:

* `upper()`
* `lower()`

Display:

* The entire string in uppercase
* The entire string in lowercase

Example:

```text
Uppercase: PYTHON PROGRAMMING IS FUN!
Lowercase: python programming is fun!
```

Do not change the original variable permanently. Store or directly display the results created by the methods.

## Part 7: Replace Part of the String

Ask the user to enter text that should be replaced.

Example:

```text
Enter a word or character you want to replace:
```

Then ask the user to enter the replacement text.

Example:

```text
Enter the new replacement text:
```

Use the `replace()` method to create a modified version of the string.

Display:

* The original stripped string
* The modified string

Example interaction:

```text
Original string: Python programming is fun!
Text to replace: fun
Replacement text: powerful
Modified string: Python programming is powerful!
```

If the requested text does not appear in the string, the program should still run without an error. Display the resulting string and an appropriate message explaining that no matching text was found.

The replacement must be performed using `replace()`. Do not manually create the modified sentence.

## Part 8: Split the String into Words

Use the `split()` method to divide the stripped string into individual words.

Store the result in a list.

Display the complete list of words.

Example:

```text
Words: ['Python', 'programming', 'is', 'fun!']
```

Also display the number of words contained in the list.

Example:

```text
Number of words: 4
```

Use `len()` to determine the number of words. Do not manually count them.

## Part 9: Process the String with a Loop

Use a loop to process the string.

Complete at least one of the following options.

### Option A: Loop Through the Words

Use a loop to display each word from the list created by `split()`.

Number the words beginning with `1`.

Example:

```text
Word 1: Python
Word 2: programming
Word 3: is
Word 4: fun!
```

### Option B: Loop Through the Characters

Use a loop to display each character in the stripped string.

Display the index position and the character.

Example:

```text
Index 0: P
Index 1: y
Index 2: t
```

Students may complete both loop options, but only one is required.

The loop must process information from the string or word list. Do not manually create a separate output statement for every word or character.

## Part 10: Organize the Program

Create a `main()` function to control the program.

The `main()` function should manage the following sequence:

1. Display the program title.
2. Ask the user to enter a string.
3. Validate that the string is not empty.
4. Strip unnecessary spaces.
5. Display the first and last characters.
6. Display the string length.
7. Display the required slices.
8. Display uppercase and lowercase versions.
9. Ask for replacement information.
10. Display the replaced string.
11. Split the string into words.
12. Display the number of words.
13. Use a loop to process the words or characters.
14. Display a completion message.

Call `main()` to begin the program.

# Required String Operations

The program must demonstrate all the following operations:

| Operation                                | Python Feature    |
| ---------------------------------------- | ----------------- |
| Remove leading and trailing spaces       | `strip()`         |
| Find the first character                 | Positive indexing |
| Find the last character                  | Negative indexing |
| Determine the number of characters       | `len()`           |
| Extract parts of the string              | Slicing           |
| Convert to uppercase                     | `upper()`         |
| Convert to lowercase                     | `lower()`         |
| Substitute text                          | `replace()`       |
| Separate the string into words           | `split()`         |
| Process words or characters individually | Loop              |

# Example Program Interaction

The exact design may vary, but the program should behave similarly to the following:

```text
STRING MANIPULATION PROGRAM

Enter a sentence or phrase:
  Python programming is fun and useful!

Original string: "  Python programming is fun and useful!  "
Stripped string: "Python programming is fun and useful!"

STRING INFORMATION
First character: P
Last character: !
Number of characters: 37

STRING SLICES
First five characters: Pytho
Last five characters: eful!
Characters from index 2 through 6: thon

LETTER CASE
Uppercase: PYTHON PROGRAMMING IS FUN AND USEFUL!
Lowercase: python programming is fun and useful!

Enter the text you want to replace: fun
Enter the replacement text: powerful

Modified string:
Python programming is powerful and useful!

WORDS
['Python', 'programming', 'is', 'fun', 'and', 'useful!']

Number of words: 6

INDIVIDUAL WORDS
Word 1: Python
Word 2: programming
Word 3: is
Word 4: fun
Word 5: and
Word 6: useful!

String manipulation completed successfully.
```

Students should create their own prompts, headings, and output formatting.

# Required Testing

## Test 1: Sentence with Extra Spaces

Enter:

```text
  Python programming is fun and useful!  
```

Replace:

```text
fun
```

With:

```text
powerful
```

Confirm that:

* The spaces at the beginning and end are removed.
* The first character is `P`.
* The last character is `!`.
* The string length is calculated correctly.
* The required slices are displayed.
* Uppercase and lowercase versions are correct.
* `fun` is replaced with `powerful`.
* The string is split into six words.
* The loop displays every word or character.

## Test 2: Short String

Enter:

```text
AI
```

Confirm that:

* The first character is `A`.
* The last character is `I`.
* The length is `2`.
* The slicing operations do not cause an error.
* Uppercase and lowercase results are displayed.
* The loop processes both characters or the single word.

## Test 3: Numbers and Punctuation

Enter:

```text
CMP 131: Python, Strings, and Loops!
```

Confirm that:

* Numbers and punctuation are preserved.
* The first and last characters are correct.
* The string length is calculated correctly.
* The string is divided into words.
* All required methods work without errors.

## Test 4: Text That Is Not Found

Enter a word to replace that does not appear in the string.

Confirm that:

* The program does not stop with an error.
* The original string remains unchanged.
* An appropriate message is displayed.

## Test 5: Empty Input

Press Enter without entering text or enter only spaces.

Confirm that:

* The program rejects the empty entry.
* An error message is displayed.
* The user is asked to enter another string.
* The program continues after valid text is entered.

# Point Distribution

* Complete comment header and descriptive program title: 5 points
* String input, meaningful variables, and empty-input validation: 10 points
* Correct use of `strip()`: 10 points
* Correct first character, last character, and string length: 15 points
* Correct string-slicing operations: 15 points
* Correct use of `upper()` and `lower()`: 10 points
* Correct use of `replace()`: 10 points
* Correct use of `split()` and word count: 10 points
* Correct loop through words or characters: 10 points
* Clear comments, output formatting, and successful testing: 5 points

**Total: 100 points**

# Code Comments

Use comments to identify and explain the major sections of the program.

Include comments for:

* Program information header
* `main()` function
* String input
* Input validation
* Removing unnecessary spaces
* Character indexing
* String-length calculation
* String slicing
* Letter-case conversion
* Text replacement
* Splitting the string
* Loop processing
* Final output

Comments should briefly explain the purpose of each major section. They should not repeat every Python statement word for word.

# General Requirements

* Use Python to complete the program.
* Create the required `string_manipulation.py` file.
* Include and call a `main()` function.
* Use meaningful and consistent variable names.
* Validate that the entered string is not empty.
* Use the stripped string for the required operations.
* Use indexing to obtain the first and last characters.
* Use `len()` to calculate string and word-list lengths.
* Use slicing to create the required substrings.
* Use all required string methods.
* Use at least one loop to process words or characters.
* Do not manually enter results that should be calculated by the program.
* Include a complete comment header.
* Include comments explaining all major program sections.
* Use clear prompts, headings, labels, and messages.
* Complete all required testing.
* Check spelling, capitalization, grammar, and punctuation.
* Make sure the program runs without errors.
* Follow the course AI-use policy.
* Record any AI assistance in `AI-Use-Report.md`.

# Required Organization

Organize the assignment as follows:

* `Week-12`

  * `Lab-01`

    * `CMP131-Week-12-Lab-01.md`
    * `AI-Use-Report.md`
    * `src`

      * `string_manipulation.py`

# Submission Requirements

Submit or push the complete `Lab-01` folder.

The submission must include:

* `string_manipulation.py`
* `AI-Use-Report.md`

Before submitting, verify that:

* The required Python file is included.
* The filename is exactly `string_manipulation.py`.
* The program contains a complete comment header.
* The program includes and calls a `main()` function.
* The program displays a descriptive title.
* The program asks the user to enter a sentence or phrase.
* Empty or space-only entries are rejected.
* `strip()` removes leading and trailing spaces.
* The first character is obtained using indexing.
* The last character is obtained using negative indexing.
* The string length is calculated with `len()`.
* All required slices are displayed.
* `upper()` displays an uppercase version.
* `lower()` displays a lowercase version.
* `replace()` creates the modified string.
* Missing replacement text is handled appropriately.
* `split()` creates a list of words.
* The number of words is calculated correctly.
* A loop processes either the words or characters.
* All results have clear labels.
* Comments explain the major string operations.
* All required tests were completed.
* The program runs without errors.
* The AI-use report is complete.
* The latest work has been committed and pushed to GitHub.

# Suggested Git Commit Messages

* Create Week 12 Lab 1 Python file
* Add string input and validation
* Add string indexing and length operations
* Add string slicing operations
* Add uppercase and lowercase conversion
* Add string replacement operation
* Split string into words
* Add loop for string processing
* Test short and empty strings
* Improve comments and output formatting
* Complete Week 12 Python lab

---

## GitHub Starter Repository

Use the following public starter repository:

[CMP131-Week-12-Lab-01](https://github.com/ahedhli12/CMP131-Week-12-Lab-01)

### Getting Started

1. Open the starter repository using the link above.
2. Select **Use this template → Create a new repository** when the template option is available.
3. Choose your personal GitHub account as the owner.
4. Name your repository `LastName-FirstName-CMP131-Week-12-Lab-01`.
5. Set your repository to **Public**.
6. Clone your own newly created repository—not the instructor’s starter repository.
7. Open the entire cloned folder in Visual Studio Code.
8. Complete and test every required Python file.
9. Commit and push your work to GitHub.
10. Verify that your latest files appear on GitHub.
11. Complete `AI-Use-Report.md`.
12. Submit the required work through Blackboard Ultra and include your public repository link when requested.

### Required Repository Files

- `CMP131-Week-12-Lab-01.md`
- `AI-Use-Policy.md`
- `AI-Use-Report.md`
- `string_manipulation.py`

### Before You Submit

- [ ] All required Python files are in the repository root.
- [ ] Every required filename is exact.
- [ ] Each program runs successfully.
- [ ] Required tests and screenshots are complete.
- [ ] `AI-Use-Report.md` is complete and accurate.
- [ ] The latest commit is visible on GitHub.
