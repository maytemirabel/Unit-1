## Quiz 7 ##

Create a program that create 10 random password with digits and letters of length 20.

```.py
import random
password=[]
num_digits= int(input("Please input the digits you want your password to be: "))
if_symbols=input('Please type True if you would like to have digits in your password: ')

if if_symbols.title()=="True":
    for x in range(num_digits):
        digit = random.randint(48, 122)
        while 57 < digit < 65 or 90 < digit < 97:
            digit = random.randint(48, 122)
        rand_chr = chr(digit)
        password.append(rand_chr)
if if_symbols.title()!="True":
    for x in range(num_digits):
        digit = random.randint(65, 122)
        while 90 < digit < 97:
            digit = chr(random.randint(65, 122))
        rand_chr=chr(digit)
        password.append(rand_chr)
for element in password:
    print(element, end=" ")
```

Fig. 1 Proof of code
<img width="1037" alt="Screen Shot 2022-09-20 at 2 21 48" src="https://user-images.githubusercontent.com/105724334/191079039-d5dcb5c4-c4e0-44df-a890-f4b5d21a9ce9.png">
