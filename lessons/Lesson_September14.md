## Lesson - September 24 ##
Create a code that allows the user to know the color of each locker 
```.py
number_lockers = 2400
for locker in range(1, number_lockers+1, 1):
    color_code = locker % 4
    colors = ["blue", "red", "white", "yellow"]
    color = colors[color_code]

    print(f"Locker No {locker} is color {color.upper().center(50,'.')}")
```
Figure.1 Proof of program

<img width="778" alt="Screen Shot 2022-09-16 at 4 03 31" src="https://user-images.githubusercontent.com/105724334/190487962-cfdf2714-46d8-4b1e-98b8-f388ec30ce2b.png">
