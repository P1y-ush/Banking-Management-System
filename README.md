# 🏦 Banking Management System

The **Banking Management System** is a console-based application designed to simulate core banking operations such as customer account management, transactions, loan processing, and administrative oversight.  
It ensures **data security, role-based access control**, and **synchronization** using file handling, locking mechanisms, and process synchronization (using semaphores and pthreads).

---

## 🚀 Features by Role

### 👤 Customer
    - Login System (one session per user)
    - View Account Balance
    - Deposit Money
    - Withdraw Money
    - Transfer Funds
    - Apply for a Loan
    - Change Password
    - Adding Feedback
    - View Transaction History
    - Logout
    - Exit

---

### 🧑‍💼 Employee
- Login System (one session per user)
    - Add New Customer
    - Modify Customer Details
    - Process Loan Applications
    - Approve/Reject Loans
    - View Assigned Loan Applications
    - View Customer Transactions( Passbook Kind of feature)
    - Change Password
    - Logout
    - Exit

---

### 👨‍💼 Manager
◦ Login System (one session per user)
    - Activate/Deactivate Customer Accounts
    - Assign Loan Application Processes to Employees
    - Review Customer Feedback
    - Change Password
    - Logout
    - Exit

---

### 🛠️ Administrator
◦ Login System (one session per user)
    - Add New Bank Employee
    - Modify Customer/Employee Details
    - Manage User Roles
    - Change Password
    - Logout
    - Exit

---

## ⚙️ Technical Details

### 🧩 Technologies Used
- **Language:** C
- **Concurrency:** POSIX Threads (`pthread`)
- **Synchronization:** Semaphores & File Locking
- **Security:** Password encryption using `libcrypt`
- **Data Storage:** Text-based file management (Flat file database)

---

## 🖥️ Compilation & Execution

- Compile Server: gcc server.c -o server -L/lib/x86_64-linux-gnu/libcrypt.so -lcrypt -pthread
- Compile Client : gcc client.c -o client
- Debug File : To View Customer, Employee, Manager, Transaction text files.
