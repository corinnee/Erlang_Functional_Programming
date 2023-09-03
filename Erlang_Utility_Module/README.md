# Erlang Utility Project

## Description
This Erlang project contains various functions that perform different tasks. These functions are categorized into three sections, each corresponding to a specific question.

## Table of Contents
- [Purpose](#purpose)
  - [Question 1](#question-1)
  - [Question 2](#question-2)
  - [Question 3](#question-3)
- [Usage](#usage)

## Purpose
The purpose of this project is to provide a set of Erlang functions that can be used for different tasks. Each function is designed to solve a specific problem or perform a particular operation. This project was completed towards part of the 'Functional Programming' module at the University of Kent. Below is a brief description of each function and its purpose:

### Question 1
This section contains functions related to processing bids and checking their success based on a threshold.

- `pos_bids/1`: Filters out bids with non-positive values.
- `success/2`: Checks if the sum of bids is greater than, equal to, or less than a given threshold.
- `add/1`: Calculates the sum of a list of bids.
- `winners/2` and `winners_co/2`: Calculate winning bids based on a threshold.

### Question 2
This section contains functions for string manipulation and substring operations.

- `init/2`: Checks if a substring exists at the beginning of a string.
- `drop/2`: Removes the first N characters from a string.
- `subst/3`: Replaces a substring (Old) with another substring (New) in a string.
- `st_len/1`: Returns the length of a string, including empty strings.
- `sub/3`: Gets a substring from a string.
- `occurs/2`: Determines if a substring occurs in a string and returns a boolean and the position.

### Question 3
This section contains functions for checking winning conditions in noughts and crosses game scenarios.

- `isxwin/1`: Checks if a list of three elements contains three 'x' values in a row.
- `linexwin/1`: Checks if a list of lists contains a horizontal 'x' win.
- `pick/2`: Selects an element from a list by index.
- `wincol/1`: Checks if a list of lists contains a vertical 'x' or 'o' win.
- `isowin/1`: Checks if a list of three elements contains three 'o' values in a row.
- `lineowin/1`: Checks if a list of lists contains a horizontal 'o' win.

## Usage
You can use this module by importing it into your Erlang project and calling the functions as needed to perform the described tasks. Refer to the inline comments within the code for detailed explanations of each function's behaviour.



