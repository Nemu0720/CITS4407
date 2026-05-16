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

## Prompt 4

**Prompt:**  
For deleting duplicate rows in awk, can I use an array such as `seen[$0]`? Is there a simpler or more readable way to write this?

**Purpose:**  
To check the awk syntax for removing fully duplicate rows while preserving the first occurrence.

# Prompt 5

**Prompt:**  
My output still showed many rows with the same `video_id`. Does this mean my duplicate-row check is wrong?

**Purpose:**  
To clarify the difference between fully duplicate rows and rows that share the same `video_id` but have different values in other columns.

---

## Prompt 6

**Prompt:**  
When comparing my cleaned CSV with the reference cleaned CSV, the files still looked different. How can I compare them while ignoring case differences and hidden carriage-return characters?

**Purpose:**  
To debug file-format and comparison issues. I learned to use commands such as `cat -vet`, `tr -d '\r'`, `tr 'A-Z' 'a-z'`, `sort`, and `diff` to check whether differences came from cleaning logic or from formatting/case differences.