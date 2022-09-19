## Quiz 8 ##
```.py
index=int(input("please input your room index from 1-100: "))
if index<0 or index>100:
    index = int(input("please put a valid room index from 1-100: "))
for floor in range(1,11,1):
    for room in range(1,11,1):
        if index==(floor-1)*10+room:
            print(f'Floor{floor} Room{room}')
```

Figure.1 Flowchart
![IMG_2502B29F9262-1](https://user-images.githubusercontent.com/105724334/191080260-9a37f9df-b032-418e-b81e-0ba276b58076.jpeg)

Figure.2 Proof of program
<img width="1053" alt="Screen Shot 2022-09-20 at 2 23 06" src="https://user-images.githubusercontent.com/105724334/191078703-c9f819d5-b329-40b1-9a0d-90a583530c38.png">
