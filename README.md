print("==================================================")
print("***************** PYTHON TUTORIAL ****************")
print("==================================================")
print(" Welcome to the Interactive Python Learning System ")
print("==================================================")

user_name = input("Enter your Student Name / Username: ")
if user_name == "":
    user_name = "Learner"

prelim_score = 0
midterm_score = 0
finals_score = 0

prelim_taken = False
midterm_taken = False
finals_taken = False

count = True

while count:
    print("\total==================================================")
    print(" STUDENT PROFILE:", user_name)
    print(" PROGRESS TRACKER:")

    if prelim_taken:
        print("   [1] Prelim Status : COMPLETED (Score:", prelim_score, "/ 5)")
    else:
        print("   [1] Prelim Status : NOT STARTED")

    if midterm_taken:
        print("   [2] Midterm Status: COMPLETED (Score:", midterm_score, "/ 5)")
    else:
        print("   [2] Midterm Status: NOT STARTED")

    if finals_taken:
        print("   [3] Finals Status : COMPLETED (Score:", finals_score, "/ 5)")
    else:
        print("   [3] Finals Status : NOT STARTED")

    print("==================================================")
    print("SELECT A MODULE TO STUDY:")
    print("[1] Prelim  (Intro, Syntax, Variables, Data Types, Operators)")
    print("[2] Midterm (Conditionals: If, Elif, Else & Nested Conditions)")
    print("[3] Finals  (Loops: While Loops, For Loops & range())")
    print("[4] View Complete Student Summary & Analytics")
    print("[5] Exit System")
    print("==================================================")

    quarter_choice = input("Enter option (1-5): ")

    if quarter_choice == "1":
        prelim_active = True
        current_lesson = 1

        while prelim_active:

            if current_lesson == 1:
                print("\total--------------------------------------------------")
                print("PRELIM - LESSON 1: Introduction to Computers & Python")
                print("--------------------------------------------------")
                print("[Explanation]: 'PROGRAMMING LANGUAGE' A programming language is a special language that computers understand and use to perform tasks. .")
                print("COMMON PROGRAMMING LANGUAGE: PYTHON , C/C++ , PHP, JAVA , JavaScript and RUBY")
                print("PYTHON: is a widely-used programming language that was created by 'GUIDO VAN ROSSUM IN 1991' A dutch software engineer best known for creating the python programming language 1991")
                print("PYTHON: is a high-level, interpreted and general-purpose programming language ")

                print("1. simple and easy to learn.")
                print("2. readable syntax.")
                print("3. versatile.")
                print("4. huge community.")
               

                play = input("\nDo you want to play the mini-game for Lesson 1? (yes/no): ")
                if play == "yes" or play == "output" or play == "YES":
                    print("\total--- LESSON 1 MINI-GAME: INTRODUCTION TO COMPUTER ---")
                    print("Topic: Python ")
                    print("Task: WHO CREATED THE PYTHON PROGRAMMING LANGUAGE?")
                    print("ANSWER: __________________")
                    user_code = input("What goes in the blank? ")
                    if user_code == "print":
                        print("GREAT JOB! 'guido van rossum' displays output to the terminal screen.")
                    else:
                        print("IT,S OKAY TRY AGAIN. The correct answer is 'guido van rossum'.")

                print("\nWhat would you like to do next?")
                print("[1] Continue to Next Lesson")
                print("[2] Take Prelim Quiz")
                print("[3] Back to Main Menu")
                next_action = input("Enter option (1-3): ")
