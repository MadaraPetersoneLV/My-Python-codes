# Python-codes-selfmade and for learning

## coin toss game - first draft
```py
import random

print("Play COIN TOSS game")

correct_guesses = []
total_number_of_guesses = []

while True:
  heads_or_tails = random.randint(0, 1)
  print(f"Heads or tails coin flip: {heads_or_tails}") # will be hidden later

  guess = input("heads (1) or tails (0) or 'stop' to quit: ")
  
  if guess == "stop":
    print("Game stopped.")
    break

  elif guess == heads_or_tails:
    print("Yes")
    continue

  else:
    print("No")
    continue
```

## import, while True, try-except, continue, count list
```py
import random
random_number = random.randint(1, 101)
print(f"Random number is: {random_number}")

number_of_guesses = []

while True:
  guess = input('guess number 1-100. Quit = stop ')

  if guess == "stop":
    print("stop game")
    break
  
  try:
    guess = int(guess)
  except:
    print("enter a number or STOP")
    continue
  number_of_guesses.append(guess)

  if guess == random_number:
    print("correct")
    break

  else:
    if guess > random_number:
      print("lower")
    else:
      print("higher")
  
  print(f"Times guessed: {len(number_of_guesses)}")
```

## Farenheit/Celsius
# Converting Farenheit/Celsius
```python
define_conversion = input('What do you want to convert? From °C or from °F (enter C or F): ')

if define_conversion == 'C':
  temperature_value_C = float(input('Enter the value in °C you want to convert: '))
  print(f'{temperature_value_C}°C equals {temperature_value_C * 9/5 + 32}°F')

else:
  temperature_value_F = float(input('Enter the value in °F you want to convert: '))
  print(f'{temperature_value_F}°F equals {(temperature_value_F - 32)/1.8}°C')
```

## Persons short profile
```python
# general information
name = "Madara"
surname = "Petersone"
age = 34
height = 1.64

print(f"Name: {name}\nSurname: {surname}\nAge: {age} \nHeight: {height}")
print()


# additional information about family
family_members = ["Didzis", "Ina", "Arturs", "Pipars", "Usins"]

print(f"Family members: {family_members}\n")

# education
bachelor_degree = True
PHD_degree = False

print("Bachelor degree: ", bachelor_degree)
print("PHD degree: ", PHD_degree),print()

favourite_movies = '"Interstellar", "Donnie Darko", "Bridge of Spies"'

print(f'Favourite movies: {favourite_movies}')
print(f'Favourite books: "Meistars un Margarita", "Trīs sivēntiņi", "Straumēni"')
```
## Guess the correct number
```python
guess_number = int(input("Try to guess the right number from 0 to 100: "))

while guess_number != 33:
    if guess_number < 33:
        print("Go up..")
        print()

    else:
        print("Go down..")
        print()

    guess_number = int(input("Try to guess the right number from 0 to 100: "))

print("CORRECT! You earn 100 hugs!!")
```

## Nori code
```python
dogs_name = input("What is your dogs name?: ")

nori_age = int(input(f"How old is {dogs_name}?: "))

if nori_age >= 2:
  print(f"{dogs_name} ir jau liels Maznodupis!")
else:
  print(f"{dogs_name} ir sīks Maznodupis.")

dogs_pets = input(f"Does {dogs_name} has any pets (yes or no)?: ")

if dogs_pets == "yes":
    number_of_pets = int(input("How many?: "))
    if number_of_pets == 1:
        one_pet_name = input("What is its name?: ")
        one_pet_nickname = input("Does it have a nickname? If yes, what is it?: ")
        if one_pet_nickname == "Pidars":
          print("hahaha. That is funny.")
          input("Is he an asshole to get such a nickname?: ")

    elif number_of_pets > 1:
        all_pet_names = input("What are their names?: ")
else:
    print("Less animals in the house - less ferr around.")
```

## BMI calculation
```python
weight = int(input("Enter your weight in kilograms: "))
height = float(input("Enter your height in meters: "))

BMI = round((weight / (height ** 2)) * 1, 2)

print(f"\nYour weight is:{weight}\nYour height is: {height}\nYour BMI is: {BMI}")
```
