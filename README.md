import random

def guess_number():
    num1=int(input("Enter the lower boundary number you want to guess ex.x-100 or y-200: "))
    num2=int(input("Enter the upper boundary number you want to guess ex.1-x or 1-y:  "))
    computer_input=random.randint(num1,num2)
    while(True):
        user_input=int(input("Now guess the number: "))
        if(user_input<computer_input):
            print("The number you enterd is too low.please try again!")
        elif(user_input>computer_input):
            print("The number you enterd is too high.please try again!")
        else:
            print("****************congratulaton You guessed The right number******************* ")
            break
            
      
guess_number()
