# Snake-Water-and-Gun-Game
The concept of this game is same as stone , paper ,scissor game and the coding of this game is easy which is based on loop, if else ,elif concept of python. 
import random
list = [' Snake' ,' Water','Gun']
choice = random.choice(list)
print(' welcome you all in Snake,Water , Gun Game!')
print(' you play this game only 10 times ')


your_wins = 0
computer_wins =0
tie = 0
no_of_games = 10

while(no_of_games>0):
    no_of_games = no_of_games - 1
    print(' You have three choices to choose\n'
          ' Press S for Snake\n'
          ' Press W for Water\n'
          'Press G for Gun\n')
    user_input = input(' Enter your choice \n')
    your_count = 0
    computer_count = 0
    tie_count =0

    if choice==' Snake':
        if user_input=='W':
            computer_count=computer_count+1
        elif user_input=='s':
            your_count=your_count+1
        else:
            tie_count=tie_count+1
    elif choice==' Water':
        if user_input=='G':
            computer_count=computer_count+1
        elif user_input=='S':
            your_count=your_count+1
        else:
            tie_count=tie_count+1
    elif choice == ' Gun':
        if user_input == 'S':
            computer_count = computer_count + 1
        elif user_input == 'W':
            your_count = your_count + 1
        else:
            tie_count = tie_count + 1

    if your_count>0:
        your_wins=your_wins+1
        print(" Mubaarak Ho aapne Computer ko haara diya h!")
    elif computer_count>0:
        computer_wins=computer_wins+1
        print('Asus jeet gya ')
    else:
        tie=tie+1
        print(' Match draw ')

print('you wins',your_wins,'times')
print('Asus wins',computer_wins,'times')
print('match draw',tie,'times')




