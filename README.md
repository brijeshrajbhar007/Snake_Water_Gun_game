# Snake_Water_Gun_game

# It is a simple but popular two person game.

# In this you need to compete with the computer.

#In this coded simple if - else function are used.

def game(a,b):
    if a == "s":
        if b == "s":
          return "It's a Draw"
        elif b == "w":
          return("computer wins")
        elif b == "g":
          return("you win")      
    elif a == "w":
        if b == "s":
          return("you win")
        elif b == "w":
          return("It's a draw")
        elif b == "g":
          return("so sad you lost")
    elif a == "g":
        if b == "s":
          return("better luck next time you 'BABY'")
        elif b == "w":
          return("by mistake you win")
        elif b == "g":
          return("It's a Draw")      


import random 

a = print("computer's turn: Snake{s} Water{w} or Gun{g}?\nDONE now it's ")
swg = random.randint(1,3)
if swg == 1:
    a = 's'
elif swg == 2:
    a = 'w'
elif swg == 3:
    a = 'g'

b = input("your turn: Snake{s} Water{w} or Gun{g}?")

print ("computer has chosen:",a,"\nand you have chosen",b )

print(game(a,b))


