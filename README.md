# ASSIGNMENT-FOR-SESSION-8
PYTHON FUNDAENTALS

#Data Type Identification

var1 = int(input('Enter your age:'))
var2 = float(input('Enter your Height:'))
var3 = str(input('Enter your name:'))
var4 = bool(input('Are you a student:'))


#Function Creation

def greet_user(name):
    return f"Welcome, {name}!"
message = greet_user("Coach")
print(message)


#Mini Login System (Input + Conditions)

def login():
    username = input("Enter username: ")
    password = input("Enter password: ")

    if username == "admin" and password == "1234":
        print("Login successful")
    else:
        print("Access denied")


#Age Categorizer


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
