# Play-n-win-snake-water-gun
import random
list=['Snake','Water','Gun']
print('choose anyone from',list)
you=0
computer=0
i=1
for i in range(10):
    choice=random.choice(list)
    player=input("choose from list ")
    print(f'computer have chosen',{choice})
    if player=='Snake' and choice=='Water':
        print('you win' )
        you=you+1
    elif player =='Water' and choice=='Snake':
        print('computer wins')
        computer+=1
    elif  player=='Water' and choice=='Water':
        print('Draw')
    elif player=='Snake'and choice=='Gun':
        print('computer wins')
        computer+=1
    elif player=='Gun' and choice=='Snake':
        print('You win')
        you=you+1
    elif player=='Gun' and choice=='Gun':
        print('Draw')
    elif  player=='Water' and choice=='Gun':
        print('You win')
        you=you+1
    elif player=='Gun' and choice=='Water':
        print('Computer wins')
        computer+=1
    elif player=='Snake' and choice=='Snake':
        print('Draw')
    else:
        print('Nobody wins')

print(you,computer)
