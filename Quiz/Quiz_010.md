## Quiz 10
#### Program code
Create a function that produces the powers of ten from pico, to tera for a number provided as an input
```.py
def powersTen (quantity: int) -> str:
    """
    Return the powers of ten of the input
    :param quantity: integer
    :return: string
    """
    out = ""
    sufix = ["unit", "kilo", "mega", "giga", "tera"]
    for power in range(4,-1,-1):
        zeros = "0"*(3*power)
        value = f"{quantity}{zeros}".ljust(25) + sufix[power]
        out += value + "\n"
    sufix = ["mili", "micro", "nano", "pico"]
    for power in range(4):
        zeros = "0"*(3*power)
        value = f"0.00{zeros}{quantity}".ljust(25) + sufix[power]
        out += value + "\n"
    return out
    
from my_library import powersTen
#test the function
ingredient_1 = input ("Insert a number: ")
out = powersTen (quantity = ingredient_1)
print (out)
```

#### Figure 1: Proof of program
<img width="1050" alt="Screen Shot 2022-10-02 at 23 51 45" src="https://user-images.githubusercontent.com/105724334/193460615-35eeec34-51ac-45bf-84e5-63fd41fb0bc5.png">

#### Figure 2: Function for program
<img width="552" alt="Screen Shot 2022-10-02 at 23 52 01" src="https://user-images.githubusercontent.com/105724334/193460619-40004580-bc86-478a-85ff-4aa1e736b0f1.png">

#### Figure 3: Flowchart 
![IMG_0410](https://user-images.githubusercontent.com/105724334/194782510-f3d2c307-806a-4415-89f0-24d73161bfc1.jpg)
