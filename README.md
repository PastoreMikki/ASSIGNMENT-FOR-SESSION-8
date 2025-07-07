# ASSIGNMENT-FOR-SESSION-8
PYTHON FUNDAENTALS

**1. Data Type Identification**
Question: Create four variables, one each for age, height, name, and whether you're a student. Print the type of each variable.


var1 = int(input('Enter your age:'))
var2 = float(input('Enter your Height:'))
var3 = str(input('Enter your name:'))
var4 = bool(input('Are you a student:'))
.
.
.
.
.
.
.
.
.



**2. Function Creation**
Question: Write a function called greet_user(name) that returns a welcome message.


def greet_user(name):
    return f"Welcome, {name}!"
message = greet_user("Coach")
print(message)

.
.
.
.
.
.
.



**3. Mini Login System (Input + Conditions)**
Question: Ask the user to enter a username and password. If the username is "admin" and the password is "1234", print "Login successful"; otherwise, print "Access denied".


def login():
    username = input("Enter username: ")
    password = input("Enter password: ")

    if username == "admin" and password == "1234":
        print("Login successful")
    else:
        print("Access denied")

.
.
.
.
.
.
.
.
.


**5. Age Categorizer**
Question: Ask the user to enter their age and print the category:0–12: Child, 13–19: Teen, 20–64: Adult, 65+: Senior


def age_category():
    try:
        age = int(input("Enter your age: "))

        if age < 0:
            print("Age cannot be negative.")
        elif age <= 12:
            print("Category: Child")
        elif age <= 19:
            print("Category: Teen")
        elif age <= 64:
            print("Category: Adult")
        else:
            print("Category: Senior")
    except ValueError:
        print("Invalid input. Please enter a valid number.")
age_category()
