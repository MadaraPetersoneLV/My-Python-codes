# My-Python-codes that I am proud of
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
