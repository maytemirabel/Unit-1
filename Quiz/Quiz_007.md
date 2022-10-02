## Quiz 7 ##
#### Program code
Create a program that create 10 random password with digits and letters of length 20.

```.py
import random
number_password = 20
password = []

for x in range(10):
    for i in range(number_password):
        rand_num = random.randint(48, 122)
        while 57 < rand_num < 65 or 90 < rand_num < 97:
            rand_num = random.randint(48, 122)
        rand_chr = chr(rand_num)
        print(rand_chr, end="")
    print(" ")
```

#### Figure 1. Proof of code
<img width="1009" alt="Screen Shot 2022-10-02 at 23 08 15" src="https://user-images.githubusercontent.com/105724334/193458346-9de96e10-5c80-4c5a-b770-ecd2067d381f.png">

#### Figure 2. Flowchart
![IMG_0398](https://user-images.githubusercontent.com/105724334/193460305-8e456ca3-80d2-43b4-a5cb-f4477609d88c.jpg)
