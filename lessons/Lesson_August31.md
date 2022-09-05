## Lesson - August 31st***

Given 2 numbers, A & B, output TRUE if one of them is 20 or if their sum is equal to 20
```.py
number_A = int(input("Enter number A: "))
number_B = int(input("Enter number B: "))
if number_A == 20 or number_B == 20 or number_B + number_A == 20:
      Output = True
else: Output = False
print(f"The solution is {Output}")
``` 

Generating 10 different emails
```.py 
name = (input("Please enter your name: "))
last_name = (input("Please enter your last name: "))
graduation_year = int(input('Please enter your graduation year: '))
x = 10
for x in range (0,10):
    print(f"Your email address is: {graduation_year}.{name}.{last_name}.{x}@uwcisak.jp")
``` 
