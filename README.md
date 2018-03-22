# 8Ball.Py
8 Ball Game

import random
import time

eight_ball = [ "It is true", "It is for sure", "No doubt", "Definitely",
               "Reliable", "Yesssss", "Very Likely", "Looks Good",
               "Yes", "Finger points to yes", "Try again", "Ask again",
               "Better not tell you now", "Cannot predict", "Concentrate on question",
               "Forget it", "No", "Spirits say no", "Not so good", "Doubtful"]

def question():
    question = input("Please ask your yes or no question to the Magic 8 Ball!\n")
    print("Predicting...")
    time.sleep(random.randrange(0,6))
    print(random.choice(eight_ball))

while True:
    question()
    repeat = input("Go ahead and ask another question? (Y or N)")
    if not (repeat == "y" or repeat == "Y"):
        print("Come back again!")
        break
