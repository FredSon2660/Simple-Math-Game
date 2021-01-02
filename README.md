# Simple-Math-Game
A small game that asks the user a math question at random
#Simple Math Game
import random

#Creating the random operator
myList = ["+", "-", "*", "/"]
i = random.choice(myList)
print(i)

#Creating the random numbers, depending on the operator
if i == "+":
  randnum1 = random.randint(0, 100)
  randnum2 = random.randint(0, 100)
  answeradd = randnum1 + randnum2
  print(randnum1, "+", randnum2)
elif i == "-":
  randnum1 = random.randint(0, 100)
  randnum2 = random.randint(0, 100)
  answersub = randnum1 - randnum2
  print(randnum1, "-", randnum2)

elif i == "*":
  randnum1 = random.randint(0, 10)
  randnum2 = random.randint(0, 10)
  answermul = randnum1 * randnum2
  print(randnum1, "*", randnum2)
elif i == "/":
  randnum1 = random.randint(1, 10)
  randnum2 = random.randint(1, 10)
  answerdiv = randnum1 / randnum2
  print(randnum1, "/", randnum2)


#Guess promt
guess = float(input("Enter your guess: "))

#Creating addition function
def add():
#  guess = float(input("Enter your guess: "))
  while answeradd == guess:
    print("Correct!")
    break
  else:
    print("False")
    while guess < answeradd:
      print("Higher")
      break
    else:
        print(("Lower"))
    print(answeradd)

#Creating subtraction function
def sub():
#  guess = float(input("Enter your guess: "))
  while answersub == guess:
    print("Correct!")
    break
  else:
    print("False")
    while guess < answersub:
      print("Higher")
      break
    else:
      print(("Lower"))
    print(answersub)

#Creating multiplication function
def mul():
#  guess = float(input("Enter your guess: "))

  while answermul == guess:
    print("Correct!")
    break
  else:
    print("False")
    while guess < answermul:
      print("Higher")
      break
    else:
      print(("Lower"))
      print(answermul)

#Creating division function
def div():
#  guess = float(input("Enter your guess: "))
  while answerdiv == guess:
    print("Correct!")
    break
  else:
    print("False")
    while guess < answerdiv:
      print("Higher")
      break
    else:
      print(("Lower"))
      print(answerdiv)

if i == "+":
  add()
if i == "-":
  sub()
if i == "*":
  mul()

if i == "/":
  div()




