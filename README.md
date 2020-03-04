# guessTheNumber

#Jonas Jason's submission (best one)

import random

secretNum = random.randint(1, 100)
score = 10

promptNum = input ("Guess a number, 1 - 100: ")
guess = int(promptNum)

while (guess != secretNum):
  if (guess < secretNum):
    print("\nScore: ",  score)
    score = score-1
    promptNum = input("Too low! Guess again: ")
    guess = int(promptNum)
  elif (guess > secretNum):
    print("\nScore: ",  score)
    score = score-1
    promptNum = input("Too high! Guess again: ")
    guess = int(promptNum)

print("\nCongratulations! You guessed correctly!")
