# rock_paper_scissors_game

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

# import the package for random situation

import random

# put the choices in the list

game_images = [rock, paper, scissors]

user_choice = int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors. \n Answer: "))

# set rules for human. 

if user_choice >= 3 or uer_choice <0:
  print("You have enter invlid number. You lose!")
else:
  print(game_images[user_choice])

  # Provide random "AI" for terminator.

  computer_choice = random.randint(0,2)

  # Let everyone knows what terminator has chosen.

  print(f"Computer has chosen {computer_choice}.")

  # Also print out the image of what the computer has chosen. 

  print(game_images[computer_choice])

  # 0 for Rock, 1 for Paper or 2 for Scissors
  # Process the results by following the official rules.

  if user_choice >=3 or user_choice < 0:
    print("You lose! You type invalid number")
  elif user_choice == 0 and computer_choice == 2:
    print("You win!")
  elif computer_choice == 0 and user_choice == 2:
    print("You lose")
  elif user_choice < computer_choice:
    print("You lose!")
  elif user_choice > computer_choice:
    print("You win!")
  elif user_choice == computer_choice:
    print("You have a draw!")






