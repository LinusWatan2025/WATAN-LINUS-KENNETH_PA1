WATAN, LINUS KENNETH C.
2ECE-A

# PYTHON PROGRAMMING EXERCISES PA1
**OVERVIEW:**
This repository contains the solutions for PA1 of the Advanced Computer Programmng and Algorightms (ECE2112) course. The project introduces fundamental Python concepts such as string manipulation, list operations, and function design. Each problem is structed to build logical thinking and coding efficiency, especially for beginners.


**PROBLEM 1: Alphabet Soup**

**What it is:**
A function that takes a string and rearranges its letters in alphabetical order.

**Why it's useful:**
This strengthens understandinng of string manipulation, sorting algorithgms, and Python's built-in functions. It's a good starting point for handling text-based data.

**How to get started:**
```python
#defining the function
def a(word):
    #using sorting function and return the alphabetized/sorted string
    return "".join(sorted(word))

#user inputs a string
w = input("Enter a string: ")
#the program calls the function
r = a(w)

#the program outputs the alphabetized form
print("Alphabetized form: ", r)
```
**Output**

<img width="264" height="23" alt="image" src="https://github.com/user-attachments/assets/5af4bb1a-dd3e-4d66-9a12-ca308f97ad73" />



**PROBLEM 2: Emoticon Converter**

**What it is:**
A function that replaces specific words (smile, grin, sad, mad) with their corresponding emoticons.

**Why it's useful:**
This exercise helps practice string replacement and conditional logic, which ae key in text processing and chat applications.

**How to get started:**
```python
#defining the function
def emotify(s):
    #dictionary assigning the given word to emoticons
    e = {
        "smile": ":)",
        "grin": ":D",
        "sad": ":(",
        "mad": ">:("
    }
    #loop to replace word in the given sentence
    for word, icon in e.items():
        #function that replaces the word to the assigned emoticon
        s = s.replace(word, icon)
    #returns the updated the sentence
    return s

#main program
#user inputs a sentence
i = input("Enter a sentence: ")
r = emotify(i)

#the programs calls the function and converts the words with their assigned emoticon
print("Converted sentence:", r)
```
**Output**

<img width="306" height="26" alt="image" src="https://github.com/user-attachments/assets/a88b1178-4b92-49ed-8838-42aff4314c9b" />




**PROBLEM 3: Unpacking List**

**What it is:**
A program that unpacks a list into three variables: first, middle, and last, wiht middle containing everything between the two ends.

**Why it's useful:**
This improves understandng of list slicing and unpacking, a common task in data handling and algorithm design.

**How to get started:**
```python
#user inputs list separated by spaces
i = input("Enter list separated by spaces: ")

#split input into a list
list = i.split()
#converts the string into integers
l = map(int, list)

#unpack into first, middle, and last
first, *middle, last = l

#print results
print("first:", first)
print("middle:", middle)
print("last:", last)
```
**Output**

<img width="182" height="54" alt="image" src="https://github.com/user-attachments/assets/618d06c2-c0b0-484f-a36e-3557174098fa" />

