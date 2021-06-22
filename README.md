# rock-paper-scissors-microbit
TRINKET IDE


import random
#we have only two players the computer and you
#we start with defining the moves r for rock s for scissors and p for paper using a list

moves=['r','s','p']
#define the winning moves based on your moves
player_wins=['pr','sp','rs']
#define the inputs
tries=0
while True: #enables the program to run forever infinitely
  player_move= input("Your Move!")
  if player_move=='q': #to quit
    break
  computer_move =random.choice(moves)
  #Output the moves
  print"You:",player_move
  print"Me", computer_move
  #using conditional
  if player_move==computer_move:
    print("It is a tie")
  elif player_move+computer_move in player_wins:
    print("You win!")
  else:
    print("You lose!")
  tries=tries+1
    
print(tries)
