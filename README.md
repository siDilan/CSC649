# CSC649 - Python Setup Experiment

## Overview
This is a simple Python program that reads a line of text entered by the user and displays both the total word count and total character count (including spaces). It gracefully handles empty inputs.

## How to Run
1. Ensure Python 3.12 is installed and the virtual environment (`.venv`) is activated.
2. Run the program via PyCharm or the terminal:
3. Enter a sentence when prompted.

## Test Results
| Test Case | Input | Expected Output |
| :--- | :--- | :--- |
| **Normal Sentence** | `Hello world this is Python` | Word count: 5, Character count: 26 |
| **Empty Input** | *(Press Enter)* | "You did not enter a sentence." |
| **Extra Spaces** | `  Hello   world  ` | Word count: 2, Character count: 18 |

## Limitation
The word count calculation splits strings by whitespace (`str.split()`). As a result, punctuation marks attached to words (e.g., `"hello,"`) are counted as part of the word rather than being stripped or isolated.