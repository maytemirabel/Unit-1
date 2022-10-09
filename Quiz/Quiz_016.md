## Quiz 16
#### Program code
Create a function that produces the output given the input shown
```.py
def BlackBoxThree (given):
    output = " "
    x = []
    for letter in given.lower():
        if letter.isalpha():
            found = False
            for element in x:
                if element [0] == letter:
                    element[1] += 1
                    found = True
                    output += str (element[1])

            if found == False: #new letter
                x.append([letter,1])
                output += "1"
        else:
            output += letter
    return output

test1 = BlackBoxThree ("hello world")
print (test1)
```

#### Figure 1: Proof of program
<img width="1024" alt="Screen Shot 2022-10-10 at 7 48 15" src="https://user-images.githubusercontent.com/105724334/194783216-8049954a-66d6-47a3-bad2-fc196840ef89.png">

#### Figure 2: Flowchart 
