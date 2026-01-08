# Guess-the-number
#A Python-based command-line number guessing game that demonstrates core programming concepts including randomization, loops, conditional logic, and user input handling. The application provides interactive feedback and tracks the number of attempts until success. 


import random

print("🎮 Welcome to the Number Guessing Game!")
number = random.randint(1, 20)
attempts = 0

while True:
    guess = int(input("Guess a number between 1 and 20: "))
    attempts += 1

    if guess < number:
        print("Too low! Try again.")
    elif guess > number:
        print("Too high! Try again.")
    else:
        print(f"🎉 Correct! You guessed it in {attempts} tries.")
        break
