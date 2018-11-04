import random
import sys
guess = ""
answer = []
numberl = []
counter = 0
print ("I'm thinking of a random 4 digit number.")
for x in range(4):
    tempnumber = random.randint(0,9)
    tempnumber = str(tempnumber)
    numberl.append(tempnumber)
number = "".join(numberl)
#print (number)
print ("Take a guess!")
def userinput():
    while True:
        global guess
        try:
            guess = input(">")
            guess = guess[:4]
            guess = str(guess)
            break
        except:
            print ("Oops, please guess a 4 digit number.")
    evaluate()
def evaluate():
    global guess
    global number
    global counter
    if number == guess:
        print (f"Correct. Well done. It took you {counter} tries. Thermonuclear war or some something...")
        sys.exit()
    for x in range(0, 4):
        global answer
        if guess[x] == number[x]:
            answer.append("Y")
        else:
            answer.append("N")
    print (f"{guess}\n{answer}")
    print ("Guess again.")
    counter += 1
    answer = []
    userinput()
userinput()
