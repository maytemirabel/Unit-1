## Lesson - September 2 ##

Create a program that calculates the tax for a salary entered by the user
```.py
print("Insert salary: ")
salary = int(input())

if not (salary < 10.000):
    tax_5 = salary * 5 / 100
    print(tax_5)

elif not (salary > 50.000):
        tax_10 = salary * 10 / 100
        print(tax_10)

elif not (salary>100.000):
        tax_15 = salary * 15 / 100
        print(tax_15)

elif not (salary>100.001):
        tax_25 = salary * 25 / 100
        print(tax_25)
```
        
Figure 1. Proof of program
<img width="1062" alt="Screen Shot 2022-09-16 at 3 28 33" src="https://user-images.githubusercontent.com/105724334/190481978-11f7a863-ba3f-43a1-b137-d8863cd45333.png">
