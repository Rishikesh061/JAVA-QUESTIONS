Customer.java:

package bank.customers;

public class Customer {

   String customerId;

   String customerName;

   String contactNumber;

   public Customer(String customerId, String customerName, String contactNumber) {

       this.customerId = customerId;

       this.customerName = customerName;

       this.contactNumber = contactNumber;

   }

   public void displayCustomer() {

       System.out.println("Customer ID = " + customerId);

       System.out.println("Customer Name = " + customerName);

       System.out.println("Contact Number = " + contactNumber);

   }

}

Loan.java:

package bank.loans;

public class Loan {

   String loanNumber;

   String loanType;

   double loanAmount;

   public Loan(String loanNumber, String loanType, double loanAmount) {

       this.loanNumber = loanNumber;

       this.loanType = loanType;

       this.loanAmount = loanAmount;

   }

   public void displayLoan() {

       System.out.println("Loan Number = " + loanNumber);

       System.out.println("Loan Type = " + loanType);

       System.out.println("Loan Amount = ₹" + loanAmount);

   }

}

Account.java:

package bank.accounts;

public class Account {

   String accountNumber;

   String accountType;

   double balance;

   public Account(String accountNumber, String accountType, double balance) {

       this.accountNumber = accountNumber;

       this.accountType = accountType;

       this.balance = balance;

   }

   public void deposit(double amount) {

       if (amount > 0) {

           balance = balance + amount;

           System.out.println("Deposited = ₹" + amount);

       } else {

           System.out.println("Invalid deposit amount");

       }

   }

   public void withdraw(double amount) {

       if (amount > 0 && amount <= balance) {

           balance = balance - amount;

           System.out.println("Withdrawn = ₹" + amount);

       } else {

           System.out.println("Insufficient balance or invalid amount");

       }

   }

   public void displayBalance() {

       System.out.println("Account Number = " + accountNumber);

       System.out.println("Account Type = " + accountType);

       System.out.println("Balance = ₹" + balance);

   }

}

Main.java:

import bank.customers.Customer;

import bank.loans.Loan;

import bank.accounts.Account;

public class Main {

   public static void main(String[] args) {

       Customer c = new Customer("C101", "Rahul", "9876543210");

       Loan l = new Loan("L201", "Home Loan", 500000);

       Account a = new Account("A301", "Savings", 20000);

       System.out.println("----- CUSTOMER DETAILS -----");

       c.displayCustomer();

       System.out.println("\n----- LOAN DETAILS -----");

       l.displayLoan();

       System.out.println("\n----- ACCOUNT DETAILS -----");

       a.displayBalance();

       System.out.println("\n----- DEPOSIT OPERATION -----");

       a.deposit(10000);

       a.displayBalance();

       System.out.println("\n----- WITHDRAWAL OPERATION -----");

       a.withdraw(5000);

       a.displayBalance();

   }

}

TEST CASE 1:

Customer ID = C101, Name = Rahul, Contact = 9876543210

TEST CASE 2:

Loan No = L201, Loan Type = Home Loan, Loan Amount = ₹500000

TEST CASE 3:

Balance increases by ₹10000

TEST CASE 4:

Withdrawal successful, Balance = ₹15000

TEST CASE 5:

Classes accessed successfully

TEST CASE 6:

Insufficient balance or invalid amount

TEST CASE 7:

Invalid deposit amount

TEST CASE 8:

Compilation error: package does not exist

TEST CASE 9:

Compilation error: Customer cannot be found

TEST CASE 10:

Compilation error: member/class is not accessible
