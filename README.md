print("==================================================")
print("*****************PYTHON TUTORIAL******************")
print("==================================================")

count = True

while count:
    print("\n==================================================")
    print("SELECT A QUARTER / MODULE TO STUDY:")
    print("[1] Prelim (Intro, Syntax, Variables, Data Types, Operators)")
    print("[2] Midterm (Conditionals: If, Elif, Else & Nested Conditions)")
    print("[3] Finals (Loops: While Loops, For Loops & range())")
    print("[4] Exit System")
    print("==================================================")
    
    quarter_choice = input("Enter option (1-4): ")

  
    if quarter_choice == "1":
        prelim_active = True
        current_lesson = 1
        
        while prelim_active:

          
            if current_lesson == 1:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 1: Introduction to Computers & Python")
                print("--------------------------------------------------")
                print("[Explanation]: A computer is an electronic device that processes data.")
                print("Python is a high-level, interpreted programming language known for its")
                print("simplicity and readability, mimicking natural human language.")
                print("[Example Code]:")
                print("   # Computers execute instructions sequentially")
                print("   print('Welcome to Computer Programming!')")
                
                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- LESSON 1 MINI-GAME: Fill in the Missing Output Code ---")
                    print("Topic: Python Output Syntax")
                    print("Task: Complete the code to output 'Python is Awesome!'.")
                    print("Code: ____('Python is Awesome!')")
                    user_code = input("What goes in the blank? ")
                    if user_code == "print":
                        print("Correct! 'print' displays output to the screen.")
                    else:
                        print("Incorrect. The correct answer is 'print'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 2
                elif next_action == "2":
                    current_lesson = 5  
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            
            elif current_lesson == 2:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 2: Variables & Syntax Rules")
                print("--------------------------------------------------")
                print("[Explanation]: A variable is a container for storing data values.")
                print("Python variable assignment uses the '=' operator. Names cannot start")
                print("with numbers and are case-sensitive.")
                print("[Example Code]:")
                print("   school_name = 'Clark College Of Science And Technology'")
                print("   student_age = 18")
                
                play = input("\nDo you want to play the mini-game for Lesson 2? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- LESSON 2 MINI-GAME: Variable Assignment ---")
                    print("Topic: Storing Data in Variables")
                    print("Task: Assign the value 100 to a variable named score.")
                    print("Code: score ____ 100")
                    user_code = input("What operator goes in the blank? ")
                    if user_code == "=":
                        print("Correct! '=' is the assignment operator.")
                    else:
                        print("Incorrect. The assignment operator is '='.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 3
                elif next_action == "2":
                    current_lesson = 5
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

            
            elif current_lesson == 3:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 3: Python Data Types")
                print("--------------------------------------------------")
                print("[Explanation]: Data types define the type of value a variable holds.")
                print("Main types: Integer (int), Floating-point (float), String (str), and Boolean (bool).")
                print("[Example Code]:")
                print("   x = 10        # int")
                print("   pi = 3.14     # float")
                print("   msg = 'Hi'    # str")
                print("   is_pass = True # bool")
                
                play = input("\nDo you want to play the mini-game for Lesson 3? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- LESSON 3 MINI-GAME: Identifying String Type ---")
                    print("Topic: Data Types (str)")
                    print("Task: Fill in the built-in type keyword for text data.")
                    print("Code: my_text = ____('Hello World')")
                    user_code = input("What data type function goes in the blank? ")
                    if user_code == "str":
                        print("Correct! 'str' represents the string data type.")
                    else:
                        print("Incorrect. The data type name is 'str'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
                
                if next_action == "1":
                    current_lesson = 4
                elif next_action == "2":
                    current_lesson = 5
                elif next_action == "3":
                    prelim_active = False
                else:
                    prelim_active = False

       
            elif current_lesson == 4:
                print("\n--------------------------------------------------")
                print("PRELIM - LESSON 4: Basic Arithmetic Operators")
                print("--------------------------------------------------")
                print("[Explanation]: Operators perform operations on variables and values.")
                print("Arithmetic includes +, -, *, /, and modulus (%) which yields division remainder.")
                print("[Example Code]:")
                print("   sum_result = 5 + 3")
                print("   remainder = 10 % 3  # Output is 1")
                
                play = input("\nDo you want to play the mini-game for Lesson 4? (yes/no): ")
                if play == "yes" or play == "y":
                    print("\n--- LESSON 4 MINI-GAME: Modulus Operator ---")
                    print("Topic: Modulus / Remainder Operator")
                    print("Task: Fill in the missing operator symbol that calculates the division remainder.")
                    print("Code: remainder = 9 ____ 4")
                    user_code = input("What operator symbol goes in the blank? ")
                    if user_code == "%":
                        print("Correct! '%' is the modulus operator.")
                    else:
                        print("Incorrect. The modulus operator is '%'.")
                
                print("\nWhat would you like to do next?")
                print("[1] Take Prelim Quiz")
                print("[2] Back to Main Menu")
                next_action = input("Enter option (1-2): ")
                
                if next_action == "1":
                    current_lesson = 5
                else:
                    prelim_active = False

       
            elif current_lesson == 5:
                print("\n--------------------------------------------------")
                print("PRELIM QUIZ (5 Questions)")
                print("--------------------------------------------------")
                score = 0
                
                print("\n1. Which function outputs text to the screen in Python?")
                print("a) display()  b) print()  c) echo()")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
                    
                print("\n2. Which of the following is a valid variable name?")
                print("a) 2nd_name  b) user-name  c) user_name")
                ans = input("Answer: ")
                if ans == "c":
                    score = score + 1
                    
                print("\n3. What data type is the value 99.5?")
                print("a) int  b) float  c) str")
                ans = input("Answer: ")
                if ans == "b":
                    score = score + 1
