# Python-rock-paper-scissors
Rock Paper Scissors 
import random
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
x=int(input("What do you choose , 0 for rock and 1 for scissors and 2 for paper?\n"))
if x == 0:
    print(rock)
elif x == 1:
    print(scissors)
elif x == 2:
    print(paper)
else:
    print("Invalid input")

y=random.randint(0,2)
print("Computer Choice:",y)
if y==0:
    print(rock)
elif y==1:
    print(scissors)
else:
    print(paper)
if (x==0 and y==1) or (x==1 and y==2) or (x==2 and y==0) :
    print("you win")
elif x==y:
    print("Draw")
else:
    print("you lose")
