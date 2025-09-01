# Metante_ProgrammingAssignment_1

# EXPERIMENT 1 - Introduction to Python Programming

# I. Intended Learning Outcomes:
1. To identify the basic codes and functions in Python Programming
2. To be able to apply the different codes and functions in creating a Python program,

# II. Instructions:
Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter
notebook in the dedicated submission bin.

# Problem #1 - ALPHABET SOUP PROBLEM
Create a function that takes a string and returns a string with its letters in alphabetical order.

a. First, Let's Define the function. 

```
def alphabet_soup(string):
```

b. Sort each characters/letters, so it will only read each letter/character and not the whole sentence/phrase.
```
 char_list = list(string)
```

c. Then, We can sort the following characters into an alphabetical order using "sorted".

```
sorted_list = sorted(char_list)
```

d. After that, we can now combine each characters into one sentence/phrase. 
```
sorted_string = ''.join(sorted_list)

    return sorted_string

```

e. Let's add an input and output for the phrase/sentence. 

```
# Input
user_input = input("Enter Sentence: ")

# Output
print(alphabet_soup(user_input))
```

## Full Code: 
```

# ALPHABET SOUP PROBLEM: 
# Create a function that takes a string and returns a string with its letters in alphabetical order.

# Start Program

# Define Function 
def alphabet_soup(string):

    # Sort Characters
    char_list = list(string)

    # Sort the list in an alphabetical order
    sorted_list = sorted(char_list)

    # Combines all the characters in one string
    sorted_string = ''.join(sorted_list)
    
    return sorted_string

# Input
user_input = input("Enter Sentence: ")

# Output
print(alphabet_soup(user_input))
```

# Problem #2 - Emoticon Problem
Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad and mad with their corresponding emoticon:

<img width="322" height="207" alt="image" src="https://github.com/user-attachments/assets/526a90aa-a030-4b29-aa8c-f3d8ed16b6bb" />


a. First, Let's Define the function. 
```
def emotify(sentence):
```

b. Let's split the sentence into a list of words, so we can determine the needed words for replacing.
```
words = sentence.split()
result = []

```

c. Let's use an If Else Statemnts to determine the words for replacing
```
for word in words:
        if word == "smile":
            result.append(":)")
        elif word == "grin":
            result.append(":D")
        elif word == "sad":
            result.append(":((")
        elif word == "mad":
            result.append(">:(")
        else:
            # keep it as is, if it does not match anything
            result.append(word)
```

d. Then, we can join it into a single string. 
```
return ' '.join(result)
```

e. Let's add an input and output for the phrase/sentence. 
```
# Input
user_input = input("Enter Sentence: ")

# Output
print(emotify(user_input))
```

## Full Code:
```
# Emoticon Problem
# Create a function that changes specific words into emoticons. Given a sentence as a string, replace the words smile, grin, sad and mad with their corresponding emoticon.

# Start Program

# Define Function
def emotify(sentence):
    # Split the sentence into a list of words
    words = sentence.split()

    # Initialize an empty list to store the converted words or emoticons
    result = []

    # Use of If Else Statement
    for word in words:
        if word == "smile":
            result.append(":)")
        elif word == "grin":
            result.append(":D")
        elif word == "sad":
            result.append(":((")
        elif word == "mad":
            result.append(">:(")
        else:
            # keep it as is, if it does not match anything
            result.append(word)

    # Joins into a single string
    return ' '.join(result)

# Input
user_input = input("Enter Sentence: ")

# Output
print(emotify(user_input))
```
# Problem #3 - UNPACKING LIST PROBLEM 
Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

a. Firstly, Let's Determine the list.
```
lst = [1, 2, 3, 4, 5, 6]
```
b. Then, we can set the code to differentiate the first, middle, and last.

B1. For the first number, we can make use of this to set the first index 0.
```
first = lst[0]
```
B2. For the last number, we can make use of this, for it will count backwards.
```
last = lst[-1] # -1, therefore it would count backward
```
B3. For the middle number/s, we can make use of this since we already know the first and last numbers. It will count the first index up until it stops to the last index.
```
middle = lst[1:-1] 
```
Full Code:
```
# UNPACKING LIST PROBLEM 
# Unpack the list writeyourcodehere into three variables, being first, middle, and last, with middle being everything in between the first and last element. Then print all three variables.

# Start Program
# List
lst = [1, 2, 3, 4, 5, 6]

# Set Code to differentiate the first, middle, and last.

first = lst[0] # first index 0

last = lst[-1] # -1, therefore it would count backward

middle = lst[1:-1] # Counts the first index (second) til it stops to the last index

# Output
print("first:", first)
print("middle:", middle)
print("last:", last)
```


# Marc Gabriel G. Metante 




