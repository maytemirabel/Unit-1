## EV Calculator ##
#### Data
```.py
date,charge,duration
12.9.22,8.878kWh,12:32:36
15.9.22,3.533kWh,5:02:23
17.9.22,6.828kWh,9:41:46
18.9.22,5.425kWh,7:43:35
```

#### Program Code
```.py
from my_library import validate_int_input, colors, bold_green, end_code

welcome_msg = " Welcome to the EV Calculator! ".center(50, "=")
prompt_msg = "Please enter an option [1-4]: "

print(f"{colors[3]}{welcome_msg}{end_code}")
print("Options".center(50))

menu = """1. Average time per kWh
2. Total kWh
3. Total charge time
4.Show all data
"""
print(menu)

def calculator():
    option = validate_int_input(prompt_msg)
    while option > 4 or option < 1:
        option = validate_int_input(f"{colors[1]}Invalid option. {prompt_msg}{end_code}")

    with open("charging_log.csv", "r") as file:
        ev_logs = file.readlines()

    # Option 1: Calculate average time per kWh
    if option == 1:
        total_time = 0
        total_kwh = 0
        i = 0
        for line in ev_logs:
            if i > 0:
                data = line.split(",")
                # print(data)
                temp_time = data[2]
                temp_time = temp_time.split(":")
                temp_time = int(temp_time[0]) * 60 + int(temp_time[1])
                total_time += temp_time
                kWh = data[1]
                total_kwh = float(kWh[0:5])
            i += 1
        print(f"{bold_green}Average time per kWh: {end_code}{colors[3]}{int(total_time / total_kwh)} minutes{end_code}")

    # Option 2: Calculate total energy
    if option == 2:
        index = 0
        total_energy = 0
        for log in ev_logs:
            if index > 0:
                values = log.split(",")
                date = values[0]
                energy = values[1]
                time = values[2]
                total_energy += float(energy[0:5])
            index += 1
        print(f"{colors[2]}The total energy charged is {total_energy}kWh{end_code}")

    # Option 3: Total charge time
    if option == 3:
        total_time = 0
        index = 0
        for line in ev_logs:
            if index > 0:
                data = line.split(",")
                time = data[2]
                time = time.split(":")
                time = int(time[0]) * 60 + int(time[1])
                total_time += time
            index += 1
        print(f"{colors[3]}Total charge time:{total_time // 60} hour(s) {total_time % 60} minutes{end_code}")

    # option 4: show all data
    if option == 4:
        print(f"{bold_green}4. Showing all data: {end_code}")
        index = 0
        for log in ev_logs:
            if index > 0:
                print(f"No.{index}: {log}", end="")  # strip removes the \n at the end of the line
            index += 1

    state = input(f"\n Do you want to view the option menu? (YES/NO): ")
    while not state.lower() in ["yes", "no"]:
        state = input(f"{state} is invalid. Do you want to view the option menu? (YES/NO): ")
    else:
        if state.lower() == "yes":
            calculator()
        else:
            goodbye = " Thank you for using EV calculator! ".center(50, "=")
            print(f"{colors[3]}{goodbye}{end_code}")
            exit()
calculator()

```

#### Figure 1. Proof of code (success)
<img width="1021" alt="Screen Shot 2022-10-08 at 3 21 04" src="https://user-images.githubusercontent.com/105724334/194625057-3e8f4e9b-ca42-4d23-a873-5e8a650a8256.png">

#### Figure 2. Proof of code (validating input)
<img width="1006" alt="Screen Shot 2022-10-08 at 3 22 00" src="https://user-images.githubusercontent.com/105724334/194625100-91d51aa2-7e5a-43ff-9ca3-7d5a6ffc1cda.png">


