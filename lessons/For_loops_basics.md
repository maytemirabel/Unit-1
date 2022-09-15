## For Loops Basics ##
1. Repeating a number multiple times in steps of 1
```.py
import random
for i in range(0, 10, 1):
    print(i)
```

2. Repeating 10 times counting from 10 down to 0
```.py
for i in range(10, -1, -1):
    print(i)
```

3. Count from 2000 to 2020 in steps of 3
```.py
for year in range(2000, 2020, 3):
    print(f"Year {year}")

for year in [2000, 2003, 2006, 2009, 2012, 2015, 2018]:
    print(f"This produces the sames years {year}")
```

4. Looping over a list of elements
```.py
for names in ["bob", "alice", "carla", "david"]:
    print(names)
```

5. Loop over letters
```.py
for let in "This is a message":
    print(let)
```

6. Loops inside a loop or Nested loops
```.py
num = 1
for row in range(3):
    for col in [0, 1, 2, 3]:
        print(str(num).center(4), end=" ")
    #printing the row
        num += 1
    print("")
```

Snakify: count number of zeros in a list
```.py
N = int(input("Enter the number of numbers to follow"))
simulated_input = []
for n in range(N):
    simulated_input.append(int(input("Enter a number")))
print(simulated_input)

num_zeros = 0
for num in simulated_input:
    if num == 0:
        num_zeros +=1
print(f"The number of zeros is {num_zeros}")
```

Rainbow of colors
```.py
end_code = "\033[00m"
for c in range(0,7):
    print(f"\033[0;3{c}m Rainbow {end_code}")

logo = '''
 ___    ___
( _<    >_ )
//        \\
\\___..___//
 `-(    )-'
   _|__|_
  /_|__|_
  /_|__|_
  /_\__/_
   \ || /  _)
     ||   ( )
Max  \\___//
      `---'
'''
print(f"\33[0;31m{logo}{end_code}")
```

7. Average lenght of words in a text
```.py
text = "Teh white small fox jumped the fence"
number_words = len(text.split(" "))
print(number_words)
sum = 0
for word in text.split(" "):
    size = len(word)
    sum += size

average = sum/number_words
print(f"The average lenght of the words in the text is {int(average)}")
```
