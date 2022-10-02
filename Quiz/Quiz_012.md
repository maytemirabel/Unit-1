## Quiz 12
#### Program code
Create a function that receives an integer 2 < N < 10, and returns the multiplication table for the number up to 9
```.py
def mulTable (i:int) -> str:
    out = " "
    for n in range (1,10):
        out+=f" {n} x {i} = {n*i}\n"
    return out
```

#### Figure 1: Proof of program
<img width="1011" alt="Screen Shot 2022-09-29 at 23 28 40" src="https://user-images.githubusercontent.com/105724334/193059171-66f5c182-a8e9-4de0-8f43-a6f460ee50a5.png">

#### Figure 2: Flowchart 
![IMG_0397](https://user-images.githubusercontent.com/105724334/193456561-54389583-ca83-4504-94f0-5c4a4adaf16a.jpg)
