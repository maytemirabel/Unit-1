## Quiz 15
#### Program code
There are N closed doors in a school and N students present. The first student opens each door. The second student flips (open⇆close) every second door. The third student flips every third door, and so on. 

Create a function that shows the doors after 5 students.
Create a function that shows the doors open after N students.

```.py
students = int (input("Input the number of students: "))
def open_doors(students):
    door = []
    for i in range(0, students):
        door.append(False)
    for i in range(0, students):
        for b in range(i, students, i+1):
            door [b] = not door [b]
    result = 0

    for i in range (students):
        if door [i] == True: result += 1
    return result
print (open_doors(students))
```

#### Figure 1: Proof of program
<img width="1032" alt="Screen Shot 2022-10-10 at 8 16 42" src="https://user-images.githubusercontent.com/105724334/194784077-9f32e9f8-dc27-4146-9677-cccbc44d9efe.png">

#### Figure 2: Flowchart 
![IMG_0414](https://user-images.githubusercontent.com/105724334/194784880-1962b22f-34cb-442d-ad1b-d1d28c27ec03.jpg)
