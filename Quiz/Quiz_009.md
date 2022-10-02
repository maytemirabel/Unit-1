## Quiz 9 ##
#### Program code
Create a function that receives as input a string and returns the string ciphered with whichever shift the user inputs

```.py
def shift_13 (msg:str) -> str:
    user_message = input (msg)
    shift = 13
    for x in range:
        range [x] = (ord(x) + shift)
        print (x)


string=input("please input your string: ").lower()
shift=int(input("please input the shift you would like to make: "))
shift = shift%26

for letter in string:
    ord_1=ord(letter)
    if ord_1==32:
        ord_2=32
    else:
        ord_2=ord_1+shift
        if ord_2>122:
            ord_2-=26
    print(chr(ord_2), end="")
```

#### Figure 1. Proof of code
<img width="1032" alt="Screen Shot 2022-10-01 at 20 25 53" src="https://user-images.githubusercontent.com/105724334/193407304-0a9b8c63-7674-45e4-9a8c-c386824d0ed8.png">

#### Figure 2. Flowchart
![IMG_0396](https://user-images.githubusercontent.com/105724334/193446482-72f88e61-8361-4e9d-99a2-8d67a5a1b103.jpg)
