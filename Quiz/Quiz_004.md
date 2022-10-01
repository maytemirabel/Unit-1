## Quiz 4
#### Program code
Based on the improved Flowchart below (Figure 2), create a program
```.py
number_1 = int (input ("Please input a number: "))
number_2 = int (number_1/10)
digit_1 = int (number_1 % 10)
digit_2 = int (number_2 % 10)
if number_1 == digit_1 + digit_2:
    print("Perfect")
else:
    print("No Perfect")
```

The purpose of this program is to check for perfect numbers: positive integers that are equal to the sum of their divisors

#### Figure 1: Proof of program
<img width="1025" alt="Screen Shot 2022-10-01 at 17 48 00" src="https://user-images.githubusercontent.com/105724334/193401338-6a6b318b-f7bd-4066-8360-d0d17a598b51.png">

#### Figure 2: Improved flowchart 
![IMG_0393](https://user-images.githubusercontent.com/105724334/193401390-54cd978d-77e4-4a78-aa36-759cc64a5cf5.jpg)
