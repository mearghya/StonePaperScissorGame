# StonePaperScissorGame
#
print("ARGHYA's STONE-PAPER-SISSOR GAME.")
import random
weapons=["STONE","PAPER","SISSOR"]
print("STONE-PAPER-SISSOR GAME")
i=0
a=0
b=0
while i<10:
    print (i+1,"th game.")
    while 1:
        print ("WEAPONS ARE:STONE,PAPER,SISSOR\n","enter your weapon\n")
        player=input()
        # print(player)
        computer=random.choice(weapons)
        print("COMPUTER:-",computer)
        if player=="SISSOR" and computer=="PAPER":
            print ("player wins.\n")
            a+=1
        elif player=="SISSOR" and computer=="STONE":
            print("computer wins.\n")
            b+=1
        elif player=="STONE" and computer=="PAPER":
            print("computer wins.\n")
            b+=1
        elif player=="STONE" and computer=="SISSOR":
            print("player wins.\n")
            a+=1
        elif player=="PAPER" and computer=="STONE":
            print("player wins.\n")
            a+=1
        elif player=="PAPER" and computer=="SISSOR":
            print("computer wins.\n")
            b+=1
        elif player==computer:
            print("Game draw.\n")
        break
    i=i+1
print("points of player=\n",a)
print("points of computer=\n",b)
if a>b:
    print("Player is match winner.\n")
elif b>a:
    print("Computer is match winner.\n")
else:
    print("Match Draw.\n")
print("Is this helpful?\n")
input()


#
