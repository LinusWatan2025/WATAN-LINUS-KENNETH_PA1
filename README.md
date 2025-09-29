## OVERVIEW

This repository contains the solutions for **PA1 of the Advanced Computer Programming and Algorithms (ECE2112)** course. The project introduces fundamental Python concepts such as **string manipulation, list operations, and function design**. Each problem is structured to build logical thinking and coding efficiency, especially for beginners.

By completing this exercise, students practice how to:

* Work with **strings** using Python’s built-in functions.
* Implement **conditional logic and replacement** with dictionaries.
* Use **list slicing and unpacking** to process sequences.

---

## PROBLEM 1: Alphabet Soup

**What it is:**

A function that takes a string and rearranges its letters in alphabetical order.

**Why it’s useful:**

This problem teaches **string sorting and manipulation**, which is a foundation for handling text-based datasets and algorithms that rely on ordering.

**How to get started:**

The program defines a function `a()` that uses Python’s built-in `sorted()` to reorder the letters of the input word, then joins them back into a string.

```python
# define a function that alphabetizes letters
def a(word):
    return "".join(sorted(word))  # sort the letters and join them

# user input
w = input("Enter a string: ")

# call the function
r = a(w)

# output the alphabetized result
print("Alphabetized form: ", r)
```

**Output:**

<img width="264" height="23" alt="image" src="https://github.com/user-attachments/assets/5af4bb1a-dd3e-4d66-9a12-ca308f97ad73" />  

---

## PROBLEM 2: Emoticon Converter

**What it is:**

A function that replaces specific words (`smile`, `grin`, `sad`, `mad`) with their corresponding emoticons.

**Why it’s useful:**

This exercise helps practice string replacement and conditional logic, which ae key in text processing and chat applications.

**How to get started:**

The program defines a dictionary that maps words to emoticons, loops through each entry, and replaces occurrences in the input sentence.

```python
# define a function for emoticon conversion
def emotify(s):
    e = {  # dictionary for mapping
        "smile": ":)",
        "grin": ":D",
        "sad": ":(",
        "mad": ">:("
    }
    for word, icon in e.items():   # loop through dictionary
        s = s.replace(word, icon)  # replace words with icons
    return s

# main program
i = input("Enter a sentence: ")  # user input
r = emotify(i)                   # convert sentence

print("Converted sentence:", r)  # display result
```

**Output:**

<img width="306" height="26" alt="image" src="https://github.com/user-attachments/assets/a88b1178-4b92-49ed-8838-42aff4314c9b" />  

---

## PROBLEM 3: Unpacking List

**What it is:**

A program that unpacks a list into three variables: **first, middle, and last**, with `middle` containing everything between the two ends.

**Why it’s useful:**

This improves understanding of **list slicing and unpacking**, which are essential in data structures, algorithms, and scenarios where elements must be separated for further processing.

**How to get started:**

The program takes a space-separated list as input, converts it into integers, and uses Python’s **extended iterable unpacking** to assign first, middle, and last values.

```python
# input list
i = input("Enter list separated by spaces: ")

# convert string into list of integers
list = i.split()
l = map(int, list)

# unpack into first, middle, last
first, *middle, last = l

# display results
print("first:", first)
print("middle:", middle)
print("last:", last)
```

**Output:**

<img width="182" height="54" alt="image" src="https://github.com/user-attachments/assets/618d06c2-c0b0-484f-a36e-3557174098fa" />  

