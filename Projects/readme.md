# Crypto Wallet: Cosmos
![](galaxy.gif)

###### Native Galaxy GIF on Tenor

## Criteria A: Planning

### Problem Definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however, at the moment she is tracking all her transactions using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms. Sato to find past transactions or important statistics about the currency. Ms. Sato is in need of a digital ledger that helps her track the amount of cryptocurrency, and the transactions, along with useful statistics.

Apart from these requirements, Ms. Sato is open to exploring a cryptocurrency selected by the developer.

## Proposed Solution

### Design statement
I will design and make a **digital ledger** for a client who **is in need of an administrative system for her cryptocurrencies: Ms. Sato**. The **ledger** will **manage all of Ms. Sato's investments and transactions as well as provide fundamental statistics about the cryptocurrency Cosmos.** The **ledger** will be constructed using the software **PyCharm** and the language **Python**, taking **3 weeks** to make. It will be evaluated according to the criteria **A and B**.

An example of the data store is:
| Date  | Category | Amount ATOMS | 
| ----- | ---------|--------------|
| 16/09/2022 | Daily | 4.35 |
| 31/09/2022 | Food | 6.73 |

The cryptocurrency that will be utilized for this project will be **Cosmos (ATOM)**. Cosmos (ATOM) is a cryptocurrency that powers an ever-expanding ecosystem of blockchains that can scale and interoperate with each other. Cosmos is a proof-of-stake chain, meaning that ATOM holders can stake their tokens in order to maintain the network and receive more ATOM as a reward.

### Rationale for Proposed Solution
The ledger that I will design begins with a welcome message and a quick description of what it does, followed by a password-protected login system in order to keep the user’s personal information safe. The user will be able to change their username and password as they please. If the login is successful, a menu with a list of actions will be displayed, asking the user what their next steps will be. After the user makes the decision, a function for that option will operate. Within the options provided, actions such as viewing past dealings, making transactions like deposits or withdrawals, and viewing information about the cryptocurrency will appear. There will be guiding messages for each step so the user will know exactly what is happening. This ledger is an effective solution because unlike other organizational methods such as spreadsheets, a digital ledger allows the user to access private information rapidly. This product is essentially the most effective solution because unlike the other tools Ms. Sato used to use, this ledger will allow her to input data concisely and organized. 

The language **Python** will be used as it is one of the most accessible programming languages available since it has simplified syntax, meaning the arrangement of words is not complicated. The additional advantage of clear syntax and easy readability is the speed of development itself. Another benefit Python has is its versatility: it can be used in a variety of environments such as mobile applications, desktop applications, web development, hardware programming, and many more.

### Success Criteria
1. The electronic ledger is text-based software (Runs in the Terminal).
2. The electronic ledger displays the basic description of the cryptocurrency selected - Cosmos.
3. The electronic ledger allows one to enter, withdraw and record transactions (including the recipient, sender, timestamp, and wallet ID of the involved stakeholders).
4. The electronic ledger is password-protected to ensure user privacy and safety.
5. The electronic ledger categorizes transactions into the different purposes ATOMS are occupied for.
6. The ledger displays the value of the cryptocurrency in different currencies. 

## Criteria B: Design

### System Diagram
![IMG_0404](https://user-images.githubusercontent.com/105724334/194106953-9c06ccbd-967f-47f6-a4bf-3101b94e9797.jpg)
#### Figure 1: System Diagram
This visual representation of how the system functions indicates the model of the computer that is being utilized as well as its descriptions such as the amount of storage it contains and its operative system. The ledger runs on Python Version 3.9.13 which is connected to a database of CSV files.

### Flow Diagrams

### Test Plan
| Test Type | Target | Procedure | Expected Outcome |
|-----------|--------|-----------|------------------|
| Functional: Unit testing | validate_int_input | 1. Use the function validate_int_input 2. Enter a letter as input 3. Enter a number as input. | 1.Error message will be print in case of letter. 2. The program will close in case of number. |
| Functional: Integrational testing | Register system | 1. Use the function register. 2. Enter a desired username and password. | After entering a desired username and password, the data will go into a database "username.csv". A message stating "Success!" will be print after the username and password have been entered.
| Functional: Integrational testing | Login system | 1. Use the function login. 2. Enter the username and password. | If the username and passwords have been stored in the database previously, the code will allow the user to continue. A message saying "Welcome back {name of user}" is expected. If the username and password entered have not been stored before, access will be denied and and the user will be asked to try again.
| Functional : Integrational testing | Record a transaction | 1. Choose to record a transaction 2. Enter the date: day, month, year 3. Choose expense category (food, daily, rent, others.) 4. Enter amount of the expense 5. The transaction will be record. | If all values have been inputed correctly (no strings in int fields) the transaction will be stored in the databse called "expenses.csv". This data will be accessible to the user using the function view past transactions. |
| Non-functional: Usuability testing | The login/register instructions and options showcased in main menu are concise and easy to follow. | 1. Run program 2. Login | The login instructions are displayed, and the main menu items can be easily read, and directions are simple to use for anyone. | 
| Non-functional: Response time | Testing if code responds quickly to user input | 1. Login to the Crypto Wallet 2. Choose any options and follow the prompted directions that follow | The code runs smoothly without crashing or severe lag. The program responds promptly to user input and displays accurate information. | 

### Record of Tasks
| Task No | Planned Action | Planned Outcome | Time estimate | Target completion date | Criterion |
|---------|----------------|-----------------|---------------|------------------------|-----------|
| 1 | write the problem definition	| A clear problem definition on Github	| 15 minutes | Sep 23 | A |
| 2 | Write down success criterias | A clear success criteria that is fitting for the problem and the client| 15 minutes | Sep 23 | A |
| 3 | Write down a proposed solution for the client| A clear justification is provided that suits the client and developer.| 15 minutes | Sep 23 | A |
| 4 | Create system diagram | Gives an idea of the hardware and software requirements | 45 minutes | Sep 25| B | 
| 5 | Create a registration and login system | The program is secured as it requires the user to register and login to their digital ledger using a username and password they set up | 1 hour | Sep 27| C | 
| 6 | Code the menu of the Crypto Wallet | Menu system that includes the title and menu items | 30 minutes | Sep 30 | C |
| 7 | Code menu options and allow user interaction | The user can pick what their next action will be from the different options from the menu. | 2 hours | Oct 3 | C | 
| 8 | Show the correct balance after money is either deposited or withdrawn | Program a function that will display the correct balance after the user has either withdrawn or deposited money| 3 hour | Oct 3 | C |
| 9 | Code transaction program | Create a code that lets the user record transactions for expenses. For example, the kind of transaction, amount and date will be asked. The data will be saved in a datase and later on will be available to the user.  | 3 hour | Oct 4 | C |
| 10 | Ensure all user input is appropiate for the requirements | Program functions that will ensure the inputs fulfil what is asked. | 2 hours | Oct 6 | C | 
| 11 | Draw and describe the flow diagrams | Provide an explanation for the drawn out flow diagrams | 2 hours | Oct 6 | B |
| 12 | Write the test plans | Expected outcomes and solutions to errors are described | 2 hours | Oct 7 | B |
| 23 | Meet with client | Seek feedback from the client about the current state of the product | 30 minutes | Oct 7 | B | 
| 21 | Finalize criteria C| Finish off explaining what skills were utilized | 2 hours | Oct 7 | C |

## Criteria C: Development
## User Acess

```.py
from my_library import validate_int_input, colors, bold_green, end_code, bold_blue

# welcome!
welcome_msg = f"{bold_blue} WELCOME TO YOUR DIGITAL LEDGER - COSMOLOGY ! {end_code}".center(110, "✧")

description_msg = "\n Cosmology is a digital ledger aiming to keep your finances organized concisely and safely. " \
                  "\n We believe it will guide you as you navigate through the world of Cosmos; your cryptocurrency. \n\n"

# import pyfiglet module
import pyfiglet
result = pyfiglet.figlet_format("C O S M O S", font = "3-d").center(100)
print(welcome_msg, description_msg, result)

prompt_msg = "Please enter an option [1-2]: "

print(f"{colors[2]}Login if you already have an account or register to create one{end_code}".center(105))

entering_menu = """1. Login
2. Register
"""
print(entering_menu)

def accesing():
    option = validate_int_input(prompt_msg)
    while option > 2 or option < 1:
        option = validate_int_input(f"{colors[1]}Invalid option.{end_code} {prompt_msg}")

    with open("username.csv", "r") as file:
        file = file.readlines()

    # Option 1: login
    if option == 1:
        print(f"{colors[4]}1. Log-in {end_code}")
        username = input("Enter your username: ")
        password = input("Enter your password: ")

        for line in file:
            line = line.strip()
            line=line.split(",")
            if username==line[0] and password==line[1]:
                print(f"Welcome back, {username}!")
                ledger()
        else:
            print(f"{colors[1]}Invalid username or password. Try again or register if you haven't.{end_code}")
            accesing()

    # Option 2: register
    if option == 2:
        print(f"{colors[4]}2. Register{end_code}")
        username = input("Create username: ")
        password = input("Create password, it must be longer than 6 characters: ")
        password_con = input("Confirm password: ")
        if len(password) <= 6:
                print(f"{colors[1]}Password is too short. Try again.{end_code}")
                accesing()
        else:
            if password != password_con:
                print(f"{colors[1]}Error! Passwords don't match. Try again.{end_code}")
                accesing()

            if username in file:
                print(f"{colors[1]}Error! Username already exists. Try again.{end_code}")
                accesing()

        with open("username.csv", "w") as file:
            #data = [username,password]
            file.write(f'{username},{password}')
        print(f"{colors[3]}Success!{end_code}")
        ledger()
accesing()
```
At the very beginning, the user is welcomed to the ledger and given two options, to login in if they have a pre existing account or to register if they do not. This code allows the user to do both. If registering, the user chooses their desired username and password, and they are also asked to confirm this password to see if they match. If all password requirements are satisfied, meaning the password is longer that 6 characters and neither the username nor the password have ever been inputed into the database "username.csv" before, the creditials of that user will be saved and stored into that said database. If the user is logging in, the program expects the user to input credentials that have been registered before and have been therefore found in the database. If they have, the user will proceed into the ledger but if they have not, the user will be asked to try again or to register if they haven't and they pressed loggin by mistake. 

## Video of the Program
[Video of the Program](https://drive.google.com/file/d/1ZUzw6oEtKnRyDeC0dIwuSIvULnd2qX/view?usp=sharing)
