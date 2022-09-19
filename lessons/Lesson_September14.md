## Task 1 - Computational Thinking ##

**Question 1: What is the most powerful computer? Glad you asked. Watch this video about Sierra Computer. Describe below points that surprised you the most.**
   * Sierra Computer is as large as 7000 square feet
   * Airblocked
   * A computer working on its own with the 'mere' purpose of storing classified data

**Question 2: Supercomputers are currently used to investigate solutions to real life problems from cancer research, Ai, economics, or brain simulation. Military uses are also one major force behind the development of these machines. Analyze the benefits and possible drawbacks of developing supercomputers in our modern world? Should we do it?**

Advantages: 
Cost-effective: Using supercomputers speeds up work management for corporations. Looking at this in a long run, it not only results in higher productivity but also lower costs. The existence of such supercomputers also means that businesses do not need to spend money on pricey physical models since this technology negates this need. 

Speed: A supercomputer performs operations much more quickly than a regular computer. Therefore, a supercomputer might complete a task in a couple of seconds  that would often take a conventional computer hours.

Disadvantages: 
Upkeep: A skilled and knowledgeable team of experts must keep an eye on and oversee a supercomputer.

High heat release: A supercomputer has multiple processors, which are capable of producing a significant amount of heat when it is in operation. Considering such temperatures, a proper cooling system muyst be installed in order to avoid any damage.


**Question 3: Identify the most advanced computer in your Country (What, specs, location, uses).**
In San Miguel Ameyalco, State of Mexico, the Abacus of Cinvestav can be found. It is equipped with 250 teraFLOPS of processing. 
    

**Programming task:**
**In a school, there are 2400 students and each student uses one locker. Each locker has a unique number from 1 to 2400. The lockers are to be painted in four colors: red, white, yellow, and blue, in order of locker numbers, as shown in the following table.** 

**Task 1: Create a program and the flow diagram that shows the colors of all the lockers from 1 to 2400**

```.py
number_lockers = 2400
for locker in range(1, number_lockers+1, 1):
    color_code = locker % 4
    colors = ["blue", "red", "white", "yellow"]
    color = colors[color_code]

    print(f"Locker No {locker} is color {color.upper().center(50,'.')}")
```
Figure.1 Proof of Task 1

<img width="778" alt="Screen Shot 2022-09-16 at 4 03 31" src="https://user-images.githubusercontent.com/105724334/190487962-cfdf2714-46d8-4b1e-98b8-f388ec30ce2b.png">

**Task 2: Using the program above, create another program that allows the user to enter a number and the program outputs the color that should be used in the locker. Create a code that allows the user to know the color of each locker**

```.py
colors =['red', 'white', 'yellow', 'blue']
locker_number = int(input('please input your locker number from 1 to 2400: '))

if locker_number<0 or locker_number>2400:
    locker_number = int(input('please input your locker number from 1 to 2400: '))
color=colors[locker_number % 4 -1]

print(f'Your locker is {color.upper()}')
```
Figure.2 Proof of Task 2
<img width="1051" alt="Screen Shot 2022-09-20 at 1 32 32" src="https://user-images.githubusercontent.com/105724334/191067692-d2a0a38a-dd68-44e3-a708-55954efc0ea5.png">
