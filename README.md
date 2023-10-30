# Rock-paper-scissors.
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

#Write your code below this line 👇

user_choice = int(input("Choose 0 for rock , 1 for paper and 2 for scissors"))
computer_choice = random.randint(0, 2)

if user_choice == 0:
    print("Your Choice", rock)
elif user_choice == 1:
    print("Your Choice",paper)
else:
    print("Your Choice", scissors)

if computer_choice == 0:
    print("Computer chooses ", rock)
elif computer_choice == 1:
    print("Computer chooses ", paper)
else:
    print("Computer chooses ", scissors)

if computer_choice > user_choice:
    print("Computer Wins")
elif user_choice == 2 and computer_choice == 0:
    print("Computer Wins")
elif user_choice == computer_choice:
    print("Game Draws")
else:
    print("You Wins")
