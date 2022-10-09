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
| Functional : Integrational testing | Record a transaction | 1. Choose to record a transaction 2. Enter the date: day, month, year 3. Choose expense category (food, daily, rent, others.) 4. Enter amount of the expense 5. If all values have been inputed correctly (no strings in int fields) the transaction will be stored in the databse called "expenses.csv". This data will be accessible to the user using the function view past transactions. |
| Non-functional: Usuability testing | The login/register instructions and options showcased in main menu are concise and easy to follow. | 1. Run program 2. Login | The login instructions are displayed, and the main menu items can be easily read, and directions are simple to use for anyone. | 
| Non-functional: Response time | Testing if code responds quickly to user input | 1. Login to the Crypto Wallet 2. Choose any options and follow the prompted directions that follow | The code runs smoothly without crashing or severe lag. The program responds promptly to user input and displays accurate information. | 

### Record of Tasks
| Task No | Planned Action | Planned Outcome | Time estimate | Target completion date | Criterion |
|---------|----------------|-----------------|---------------|------------------------|-----------|
| 1 | Meet withe the client | Talk with the client to dicuss the problems they are facing and brainstorm solutions to create a plan to help the client resolve the problems| 10 minutes | Sep 23 | A |
| 2 | Brainstorm and write the problem definition	| A clear problem definition on Github	| 15 minutes | Sep 23 | A |
| 3 | Brainstorm and write down success criterias | A clear success criteria that suits the client and resolves the problem | 15 minutes | Sep 23 | A |
| 4 | Brainstorm and write down a proposed solution for the client| A clear justification that suits the client and developer.| 15 minutes | Sep 23 | A |
| 5 | Create system diagram | To have a clear idea of the hardware and software requirements for the proposed solution | 45 minutes | Sep 23| B | 
| 6 | Create a simple registration and login system | To create a program that allows the user to register and login to their digital ledger using a username and password they set up | 1 hour minutes| Sep 26| C | 
| 7 | Encrypt the password | A program to protect the application using a password with encryption | 45 minutes | Sep 28 | C |
| 8 | Code the menu of the Crypto Wallet | To have a menu system that includes the title and menu items on the screen | 20 minutes | Sep 30 | C |
| 9 | Code menu options and allow user interaction | The user can choose different options from the menu (Ex: Option 1: Record transcation, and the user will be able to choose Option 1 to record a transaction). | 2 hours | Oct 1 | C | 
| 10 | Create visual display of expense data | Code a bar graph that includes all expense history in categories. | 20 minutes | Oct 1 | C |
| 11 | Create a visual display for transaction data | Code a chart that includes all transaction data with the date, expense, and amount. | 45 minutes | Oct 2 | C |
| 12 | Code a menu for deposit and withdraw | Code a second menu that gives the user two options: Deposit and Withdraw. | 15 minutes | Oct 2 | C |
| 13 | Display correct balance after money is either deposited or withdrawn | Code a function that would add or subtract the amount of money deposited or withdrawn from the balance and print the updated balance | 1 hour | Oct 3 | C |
| 14 | Code a menu for creating or viewing transactions | Code a second menu that gives the user two options: Create a transaction, View transaction history. | 15 minutes | Oct 4 | C |
| 15 | Code transaction functions | Create a code that allows the user to record when they made the transaction, what kind of transaction it was, and how much the transaction was. The code will then transfer all of that information into a spreadsheet and bar graph, with accurate data | 1 hour | Oct 4 | C |
| 16 | Make sure to validate user input for all option choices | Code functions that would make sure what the user inputs follows the requirements (Ex: If a number digit is required but user enters a character, an error message will print, and allowing them to retry). | 1 hour 30 minutes | Oct 5 | C | 
| 17 | Hide the password when it is being typed | The user will only see asteriks when entering their password to increase security. | 45 minutes | Oct 5 | C |
| 18 | Draw and describe the flow diagrams | Flow diagrams for different parts of the solution along with a brief explanation | 1 hour | Oct 6 | B |
| 19 | Write the test plans | Procedures one should take to test the program and the expected outcome of each test is on Github | 1 hour | Oct 7 | B |
| 20 | Meet with client | Hear feedback from the client about the current state of the product | 30 minutes | Oct 7 | B | 
| 21 | Finish Criteria C | Write the descriptions of the code and the detail of the techniques that were used on Github | 2 hours | Oct 7 | C |

## Criteria C: Development
## User registration

```.py
def register(uname:str, password:str):
    '''
    This function saves a user, password in the file
    credentials.csv
    :param uname: username a string
    :param password: password a string
    :return: nothing
    '''
    #open the file in mode append: a
    file = open("credentials.csv", "a")
    salty = "¯\(°_O)/¯"
    to_hash = uname + password + salty
    hashed_password = hmac.new(''.encode(), to_hash.encode(), 'sha512').hexdigest()
    file.write(f"{uname},{hashed_password}\n")
```

The first part of creating a digital ledger for a client is to create a registration system so the client can create a Crypto Wallet account. This code allows the user to enter a username and password they desire, and it adds their crendentials into a file with and encrypted password. The encryption I used in this is called "hashing". Encryption is the process of encoding plain text or any information in such a way that only authorized people can read it with a corresponding key, like a password, so that confidential data can be protected from unauthorized persons. Hashing converts any amount of data into a fixed-length hash that cannot be reversed. In my code, it is hashed using a random string of characters, known as a salt. This is an additional input to my code above to hash the user's password.

## Video of the Program
[Video of the Program](https://drive.google.com/file/d/1ZUzw6oEtKnRyDeC0dIwuSIvULnd2qX/view?usp=sharing)
