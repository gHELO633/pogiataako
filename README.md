print("==================================================")
print("***************** PYTHON TUTORIAL ****************")
print("==================================================")
print("   Welcome to the Python Learning Tutorial System   ")
print("==================================================")

student_name = input("Enter your student name / username: ")
if student_name == "":
    student_name = "Learner"

prelim_score = 0
midterm_score = 0
finals_score = 0

prelim_taken = False
midterm_taken = False
finals_taken = False

count = True

while count:
    print("\n==================================================")
    print(f" STUDENT PROFILE: {student_name}")
    print(" PROGRESS TRACKER:")

    if prelim_taken:
        print(f"   [1] Prelim Status : COMPLETED (Score: {prelim_score} / 5)")
    else:
        print("   [1] Prelim Status : NOT STARTED YET")

    if midterm_taken:
        print(f"   [2] Midterm Status: COMPLETED (Score: {midterm_score} / 5)")
    else:
        print("   [2] Midterm Status: NOT STARTED YET")

    if finals_taken:
        print(f"   [3] Finals Status : COMPLETED (Score: {finals_score} / 5)")
    else:
        print("   [3] Finals Status : NOT STARTED YET")

    print("==================================================")
    print("SELECT A MODULE TO STUDY:")
    print("[1] Prelim  (Intro, Syntax, Variables, Data Types, Operators)")
    print("[2] Midterm (Conditionals: If, Elif, Else & Nested Conditions)")
    print("[3] Finals  (Loops: While Loops, For Loops & range())")
    print("[4] View Complete Student Summary & Analytics")
    print("[5] Exit System")
    print("==================================================")

    term_choice = input("Enter option (1-5): ")

    if term_choice == "1":
        prelim_latest = True
        current_lesson = 1

        while prelim_latest:
            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("PRELIM - Introduction to Computers & Python")
                print("--------------------------------------------------")
                print("[Explanation]: A programming language is a special language used to communicate with computers.")
                print("Common programming languages include Python, C++, PHP, Java, JavaScript, and Ruby.")
                print("Python is widely used because it is easy to learn, readable, and versatile.")
                print("Python was created by Guido van Rossum in 1991.")
                print("Python is a high-level, interpreted, general-purpose programming language.")
                print("Why learn Python?")
                print("1. Simple and easy to learn")
                print("2. Clean and readable syntax")
                print("3. Very versatile")
                print("4. Large community support")

                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 1 MINI-GAME: INTRODUCTION TO PYTHON ---")
                    print("Topic: Python Basics")
                    print("Task: Who created the Python programming language?")
                    print("Answer: __________________")
                    user_answer = input("What goes in the blank? ").lower()
                    if user_answer == "guido van rossum":
                        print("GREAT JOB! Guido van Rossum is the correct answer.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is 'Guido van Rossum'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 2
                elif next_input == "2":
                    current_lesson = 5
                elif next_input == "3":
                    prelim_latest = False
                else:
                    prelim_latest = False

            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("PRELIM - Basic Syntax")
                print("--------------------------------------------------")
                print("[Explanation]: A variable is a container used to store data values.")
                print("Python uses the '=' operator for assignment.")
                print("Variable names cannot start with numbers and are case-sensitive.")
                print("Example code: name = 'John'")
                print("print(name) - prints the value of the variable")
                print("Indention matters in Python because it defines code blocks.")
                print("Example: if age >= 18:")
                print("    print('Adult')")
                print("Example code: print('HELLO, WORLD!')")
                print("Example code: print(100)")
                print("Python comments can be written using '#'.")
                print("Example: # This is a single-line comment")

                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 2 MINI-GAME: VARIABLE ASSIGNMENT ---")
                    print("Topic: Storing Data in Variables")
                    print("Task: Assign the value 100 to a variable named score.")
                    print("Code: score ____ 100")
                    user_answer = input("What operator goes in the blank? ")
                    if user_answer == "=":
                        print("GREAT JOB! '=' is the correct answer.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is '='.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 3
                elif next_input == "2":
                    current_lesson = 5
                elif next_input == "3":
                    prelim_latest = False
                else:
                    prelim_latest = False

            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("PRELIM - Python Data Types")
                print("--------------------------------------------------")
                print("[Explanation]: Data types define the kind of data a variable can hold.")
                print("Main types: Integer (int), Floating-point (float), String (str), and Boolean (bool).")
                print("Example code:")
                print("   element = 10")
                print("   pi = 3.14")
                print("   msg = 'Hi'")
                print("   is_pass = True")

                play = input("\nDo you want to play the mini-game for Lesson 3? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 3 MINI-GAME: IDENTIFYING STRING TYPE ---")
                    print("Topic: Data Types (str)")
                    print("Task: Fill in the built-in type keyword for text data.")
                    print("Code: my_text = ____('Hello World')")
                    user_answer = input("What data type goes in the blank? ")
                    if user_answer == "str":
                        print("GREAT JOB! 'str' represents the string data type.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The correct answer is 'str'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_input = input("Enter option (1-3): ")

                if next_input == "1":
                    current_lesson = 4
                elif next_input == "2":
                    current_lesson = 5
                elif next_input == "3":
                    prelim_latest = False
                else:
                    prelim_latest = False

            elif current_lesson == 4:
                print("\n--------------------------------------------------")
                print("PRELIM - Basic Arithmetic Operators")
                print("--------------------------------------------------")
                print("[Explanation]: Operators perform operations on variables and values.")
                print("Arithmetic operators include +, -, *, /, and %.")
                print("The modulus operator (%) gives the remainder after division.")
                print("Example code:")
                print("   sum_result = 5 + 3")
                print("   remainder = 10 % 3")

                play = input("\nDo you want to play the mini-game for Lesson 4? (yes/no): ").lower()
                if play in ["yes", "y"]:
                    print("\n--- LESSON 4 MINI-GAME: MODULUS OPERATOR ---")
                    print("Topic: Modulus / Remainder Operator")
                    print("Task: Fill in the missing operator symbol that calculates the division remainder.")
                    print("Code: remainder = 9 ____ 4")
                    user_answer = input("What operator symbol goes in the blank? ")
                    if user_answer == "%":
                        print("GREAT JOB! '%' is the modulus operator.")
                    else:
                        print("IT'S OKAY TRY AGAIN. The modulus operator is '%'.")

                print("\nWhat would you like to do next?")
                print("[1] Take Prelim Quiz")
                print("[2] Back to Main Menu")
                next_input = input("Enter option (1-2): ")

                if next_input == "1":
                    current_lesson = 5
                else:
                    prelim_latest = False

            elif current_lesson == 5:
                print("\n--------------------------------------------------")
                print("PRELIM QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0

                print("\n1. Which function outputs text to the screen in Python?")
                print("a) display()  b) print()  c) echo()")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n2. Which of the following is a valid variable name?")
                print("a) 2nd_name  b) user-name  c) user_name")
                ans = input("Answer: ").lower()
                if ans == "c":
                    score += 1

                print("\n3. What data type is the value 99.5?")
                print("a) int  b) float  c) str")
                ans = input("Answer: ").lower()
                if ans == "b":
                    score += 1

                print("\n4. What is the output of 10 % 3?")
                print("a) 3  b) 0.33  c) 1")
                ans = input("Answer: ").lower()
                if ans == "c":
                    score += 1

                print("\n5. Which symbol is used for single-line comments in Python?")
                print("a) #  b) //  c) /*")
                ans = input("Answer: ").lower()
                if ans == "a":
                    score += 1
