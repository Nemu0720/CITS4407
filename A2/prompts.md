#This document recors selected AI promopts used during Assignment 2.

## Prompt 1

**Prompt:**  
Help me polish the wording of my `prompts.md` file so that it clearly states the AI was used for syntax checking, debugging support, and grammar improvement?

**Purpose:**  
To improve the grammar and clarity of the AI prompt log.

## Prompt 2

**Prompt:**  
For the anti-bugging part of Question 1, should I use `-f` or `-d` to check whether the input file exists?

**Purpose:**  
To check the correct Bash file test syntax. I learned that `-f` checks for an ordinary file, while `-d` checks for a directory.

## Prompt 3

**Prompt:**  
My variable `col_number` is empty after running this command:  
`col_number=$(head -n 1 "$1" | awk -F, '{printNF}')`  
Why is it empty?

**Purpose:**  
To debug an awk syntax error. I learned that `print NF` needs a space between `print` and `NF`; otherwise, awk treats `printNF` as a variable name.