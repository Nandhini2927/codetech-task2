**name** Nandhini M
**id** CT08DS728
**domain** JAVA PROGRAMMING
**duration** AUGUST 30 TH 2024 TO SEPTEMBER 30 TH 2024
**mentor** Neela Santhosh Kumar
objective:
The objective of the OnlineBankingSystem program is to create a simple command-line banking application that allows users to manage their bank accounts through various operations such as creating accounts, depositing funds, withdrawing funds, transferring money between accounts, and viewing transaction histories.
about the program:
Account Class:

Attributes:
accountNumber: Unique identifier for the account.
owner: Name of the account holder.
balance: Current balance of the account.
transactionHistory: A list to keep track of all transactions (deposits, withdrawals, transfers).
Methods:
Constructor: Initializes the account with the account number and owner, setting the balance to zero.
deposit(double amount): Increases the balance and records the transaction.
withdraw(double amount): Decreases the balance if sufficient funds are available and records the transaction; returns a boolean indicating success or failure.
transfer(Account toAccount, double amount): Transfers funds between accounts, using the withdraw and deposit methods.
getTransactionHistory(): Returns the transaction history for the account.
BankingSystem Class:

Attributes:
accounts: A map that stores all accounts, keyed by account number.
Methods:
createAccount(String accountNumber, String owner): Creates a new account if it doesn’t already exist.
getAccount(String accountNumber): Retrieves an account based on the account number.
deposit(String accountNumber, double amount): Calls the deposit method on the specified account.
withdraw(String accountNumber, double amount): Calls the withdraw method on the specified account.
transfer(String fromAccountNumber, String toAccountNumber, double amount): Manages fund transfers between accounts.
viewTransactionHistory(String accountNumber): Displays the transaction history for the specified account.
OnlineBankingSystem Class:

This is the main class containing the main method, which runs the application.
It provides a user interface via a command-line menu that allows users to interact with the banking system.
The program runs in a loop, prompting the user to select an option until they choose to exit.
