# **Banking Management System (BMS)**

Welcome to the **Banking Management System (BMS)**! This is a simple yet powerful C++ program designed to handle basic banking operations, such as managing customer accounts, processing deposits, withdrawals, and transfers, all with a user-friendly console interface.

---

CS-112-SEMESTER-Project: Object Oriented Programming and Design 📈
---
Team Members 🌐
Muhammad Arsal - 2022350
Wardah Haya - 2022622

---

## **Features 🚀**

- **Account Search**: Search for customer accounts by **account number** or **full name**.
- **Balance Inquiry**: Check the current **account balance**.
- **Cash Deposit**: Easily deposit **cash** into a customer's account.
- **Cash Withdrawal**: **Withdraw** funds from a customer's account, with fees if applicable.
- **Money Transfer**: **Transfer funds** between accounts with ease.
- **Logout**: Safely **logout** from the system and view your logout time.

---

## **Prerequisites 🛠️**

To run the **Banking Management System**, you will need:

- **C++ Compiler**: A C++ compiler like **GCC**, or an IDE like **Code::Blocks**, **Visual Studio**, or **CLion**.
- The program uses basic C++ features like **file handling** (`ifstream` and `ofstream`), **user input/output**, and basic control flow (loops, conditionals).
- **`gotoxy()` function** for cursor positioning in the console. This requires libraries like **`conio.h`** (works on **Windows**).

---

## **File Structure 📁**

- **`record.bin`**: This binary file stores customer account records. It includes sensitive information such as account numbers, names, balances, contact info, and more.
- **`new.bin`**: A temporary file used during operations like deposits, withdrawals, or transfers to store modified records before updating the main `record.bin` file.

---

## **Functionalities Overview 💼**

### 1. **Account Search by Account Number**
   - **Search** for a customer account using the **account number**.
   - View detailed account information including name, balance, phone number, etc.

### 2. **Account Search by Name**
   - **Search** for a customer account using their **full name**.
   - View detailed account information for the matching account.

### 3. **Balance Inquiry**
   - **Check** the balance of a customer account by entering the **account number**.

### 4. **Cash Deposit**
   - **Deposit** money into a customer account by specifying the deposit amount.

### 5. **Cash Withdrawal**
   - **Withdraw** funds from a customer account. A small fee may apply if the balance exceeds a certain threshold.

### 6. **Money Transfer**
   - **Transfer** funds from one account to another.
   - Specify both the **sender’s** and **recipient's** account number and the transfer amount.

### 7. **Log Out**
   - **Logout** from the system and view the **logout time**.

---

## **How to Use 🖥️**

### Step 1: Compile the Code

1. Save the provided C++ code into a file (e.g., `bms.cpp`).
2. Compile the code using a C++ compiler. Example with `g++`:
   ```bash
   g++ bms.cpp -o bms
   ```

### Step 2: Run the Program

Once compiled, run the program with the following command:
```bash
./bms
```

### Step 3: Interact with the Program

Once the program starts, follow the **on-screen prompts** to perform banking operations such as:
- **Searching for an account**
- **Checking account balance**
- **Depositing or withdrawing cash**
- **Transferring funds between accounts**

### Step 4: Exit the Program

Press **Enter** to exit the program after completing your operations.

---

## **Example of Usage 📝**

### 1. **Login to the System**
   - Upon starting, the system will prompt you to **enter your user ID** to log in.

### 2. **Perform Banking Operations**
   - After logging in, choose from the following options:
     - Search for an account by **account number** or **name**.
     - Check the **account balance**.
     - **Deposit** or **withdraw** cash from the account.
     - **Transfer money** to another account.

### 3. **Logout**
   - You can log out at any time by selecting the **Log Out** option. The system will display the **logout time**.

---

## **File Operations & Data Integrity 💾**

- **Account records** are stored in a **binary file (`record.bin`)** for efficient data storage.
- After performing operations such as **deposit**, **withdrawal**, or **transfer**, the modified records are temporarily stored in **`new.bin`** before updating the main file.
- This ensures **data consistency** while handling customer account updates.

---

## **Error Handling ⚠️**

- The system verifies whether the entered **account number** exists before performing any operation (deposit, withdrawal, or transfer).
- If the **account doesn't exist**, the system will prompt you to enter a valid **account number**.
- If the entered withdrawal or transfer amount exceeds the available balance, the system will notify you of **insufficient funds**.
- If non-numeric values are entered (e.g., for account numbers or amounts), the system may crash or behave unpredictably.

---

## **Limitations 🚧**

- The program does not have advanced features like **encryption** or secure **user authentication**, so it is not suitable for real-world banking environments.
- The use of **`gotoxy()`** makes the program **platform-dependent** (works on **Windows** but may not work on **Linux/macOS** without additional libraries).

---

## **Future Improvements 🔮**

- **User Authentication**: Add a secure **login system** with usernames and passwords.
- **Input Validation**: Improve error handling and **input validation**.
- **Modern User Interface**: Upgrade the user interface to be more user-friendly, possibly using a **Graphical User Interface (GUI)**.
- **Transaction History**: Implement a feature to **view transaction history** for each account.
- **Data Encryption**: Add **encryption** to securely store sensitive account information.

---

## **License 📝**

This project is provided under the **[MIT License](https://opensource.org/licenses/MIT)**. Feel free to use, modify, and distribute this code as per the terms of the MIT License.
