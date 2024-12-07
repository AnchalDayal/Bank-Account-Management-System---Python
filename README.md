# Python Bank Account Management System  

## Objective  
This project is a Python-based simulation of a bank account management system. It allows users to create and manage bank accounts, perform transactions, and retrieve account details. The system demonstrates the application of fundamental Python concepts such as variables, data structures, functions, file handling, and modules.  

## Features  

### 1. Account Management  
- Create new bank accounts with the following attributes:  
  - Account holder's name  
  - Auto-generated account number (11 digits)  
  - Account type (e.g., savings or current)  
  - Initial balance  
- Retrieve account details, including:  
  - Account holder's name  
  - Account number  
  - Account type  
  - Current balance  

### 2. Transactions  
- **Deposit:** Add money to an account.  
- **Withdrawal:** Withdraw money, ensuring the withdrawal does not exceed the current balance.  
- **Transfer:** Transfer funds between two accounts with proper validation.  
- Transactions automatically update the account balances.  

### 3. File Handling  
- Persistent storage of account details and transaction history using the `pickle` library.  
- Load account data at program startup and save updates on termination.  
- Append new transactions to existing records without overwriting previous data.  

### 4. Reports  
- View transaction history for any account, displaying:  
  - Date  
  - Type of transaction (deposit, withdrawal, transfer)  
  - Amount  
  - Target account (if applicable)  
- Generate summary statistics for each account, including:  
  - Total deposits  
  - Total withdrawals  
  - Average transaction amounts (using NumPy functions)  

### 5. User Interaction  
- An interactive menu for the following operations:  
  - Open a new account  
  - View account details  
  - Perform transactions (deposit, withdraw, transfer)  
  - View transaction history  
  - Exit the program  
- Smooth navigation using conditional statements and loops.  

### 6. Error Handling  
- Input validation to ensure:  
  - Positive amounts for deposits and withdrawals.  
  - Adequate balance before withdrawal or transfer.  
- Prevent invalid operations like transferring funds between non-existent accounts.  

### 7. Bonus Features (Optional)  
- Login functionality for multiple users with username and password.  
- Advanced Python features like lambda functions for quick calculations.  

---

## Installation  

### Prerequisites  
- Python 3.8 or later  
- Required libraries:  
  - NumPy  
  - Pickle (built-in module)  

### Steps  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/python-bank-system.git  
   cd python-bank-system  
   ```  

2. Install NumPy:  
   ```bash  
   pip install numpy  
   ```  

3. Run the program:  
   ```bash  
   python bank_management.py  
   ```  

---

## Usage  

The program provides an interactive menu to perform the following operations:  
1. Open a new account  
2. View account details  
3. Deposit money  
4. Withdraw money  
5. Transfer money  
6. View transaction history  
7. View summary statistics  
8. Exit  

---

## Example  

### Account Creation  
```text  
Enter account holder's name: John Doe  
Enter account type (Savings/Current): Savings  
Enter initial balance: 5000  

Account created successfully!  
Account No: 12345678901  
User ID: john_doe8901  
Password: 123456  
```  

### Deposit  
```text  
Enter account number: 12345678901  
Enter amount to deposit: 2000  

Deposited 2000 successfully! New Balance: 7000  
```  

### Transaction History  
```text  
Date: 2024-12-07 12:34:56, Type: Deposit, Amount: 2000, Target Account: N/A  
```  

---

## Project Structure  

```  
python-bank-system/  
│  
├── bank_management.py   # Main program file  
├── accounts_data.pkl    # Stored account details  
├── transactions_data.pkl # Stored transaction history  
├── README.md            # Project documentation  
```  

---

## Future Enhancements  
- Add a graphical user interface (GUI) for improved user experience.  
- Implement real-time notifications for transactions.  
- Support for multi-currency accounts and international transfers.  

---

## Contributing  
Contributions are welcome! Feel free to fork the repository and submit a pull request.  

---

## License  
This project is licensed under the MIT License.  

---  
