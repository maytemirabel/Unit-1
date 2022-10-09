## Quiz 11
#### Program code
Create a function that shows the days of your birthday’s month for the year 2022
```.py
def bestMonth():
    month = int(input('Input the number of the month you would like to see: [1 - 12:] '))
    dayofweek = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
    day_start = [0, 4, 0, 0, 3, -2, 1, 3, -1, 2, 4, 0, 2]
    if month == 1 or month == 3 or month == 5 or month == 7 or month == 8 or month == 10 or month == 12:
        day = 32
        for i in range(1, day):
            print(i, dayofweek[(i + day_start[month]) % 7])
    elif month == 2:
        day = 29
        for i in range(1, day):
            print(i, dayofweek[(i + day_start[month]) % 7])
    else:
        day = 31
        for i in range(1, day):
            print(i, dayofweek[(i + day_start[month]) % 7])
    exit()

# ------------------
out = bestMonth()
print(out)
```

#### Figure 1: Proof of program

#### Figure 2: Flowchart 
