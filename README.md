## OVERVIEW

This repository contains the solutions for **PA1 of the Advanced Computer Programming and Algorithms (ECE2112)** course. The project introduces fundamental Python concepts such as **string manipulation, list operations, and function design**. Each problem is structured to build logical thinking and coding efficiency, especially for beginners.

---

## PROBLEM 1: Alphabet Soup

**What it is:**

A function that takes a string and rearranges its letters in alphabetical order.

**Why it's useful:**

This strengthens understanding of **string manipulation, sorting algorithms, and Python's built-in functions**. It’s a good starting point for handling text-based data.

**How to get started:**

First, define a function that takes a word as input. The built-in `sorted()` function arranges the characters alphabetically, and `"".join()` merges them back into a single string.

```python
#defining the function
def a(word):
    #using sorting function and return the alphabetized string
    return "".join(sorted(word))
```

Next, allow the user to enter a string and pass it into the function. The result is stored and then displayed.

```python
#user inputs a string
w = input("Enter a string: ")

#the program calls the function
r = a(w)

#the program outputs the alphabetized form
print("Alphabetized form:", r)
```

**Output:**

<img width="264" height="23" alt="image" src="https://github.com/user-attachments/assets/5af4bb1a-dd3e-4d66-9a12-ca308f97ad73" />  

---

## PROBLEM 2: Emoticon Converter

**What it is:**

A function that replaces specific words (smile, grin, sad, mad) with their corresponding emoticons.

**Why it's useful:**

This exercise helps practice **string replacement and conditional logic**, which are key in text processing and chat applications.

**How to get started:**

First, define a function and create a dictionary mapping words to emoticons. Using `.replace()`, each matching word in the string is replaced with its corresponding symbol.

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
        s = s.replace(word, icon)  #replace words with emoticons
    return s
```

Next, accept input from the user, call the function, and display the updated sentence.

```python
#main program
i = input("Enter a sentence: ")

#the program calls the function and converts words to emoticons
r = emotify(i)

print("Converted sentence:", r)
```

**Output:**

<img width="306" height="26" alt="image" src="https://github.com/user-attachments/assets/a88b1178-4b92-49ed-8838-42aff4314c9b" />  

---

## PROBLEM 3: Unpacking List

**What it is:**

A program that unpacks a list into three variables: **first, middle, and last**, with middle containing everything in between.

**Why it's useful:**

This improves understanding of **list slicing and unpacking**, which are common in data handling and algorithm design.

**How to get started:**

First, request a list from the user, split it into elements, and convert them into integers for processing.

```python
#user inputs list separated by spaces
i = input("Enter list separated by spaces: ")

#split input into a list and convert to integers
list = i.split()
l = map(int, list)
```

Next, unpack the list into three parts: the first element, the last element, and everything in between.

```python
#unpack into first, middle, and last
first, *middle, last = l
```

Finally, print the results to show the separation.

```python
#print results
print("first:", first)
print("middle:", middle)
print("last:", last)
```

**Output:**

<img width="182" height="54" alt="image" src="https://github.com/user-attachments/assets/618d06c2-c0b0-484f-a36e-3557174098fa" />  

