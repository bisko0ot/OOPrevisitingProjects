# OOPrevisitingProjects
ATM-Machine
// ATM.java
class ATM {
    private int balance = 10000;

    void withdraw(int amount) {
        if (amount <= balance) {
            balance -= amount;
            System.out.println("Withdrawn: " + amount);
        } else {
            System.out.println("Insufficient Balance");
        }
    }

    void checkBalance() {
        System.out.println("Balance: " + balance);
    }
}
// Main.java
public class Main {
    public static void main(String[] args) {
        ATM atm = new ATM();
        atm.checkBalance();
        atm.withdraw(3000);
        atm.checkBalance();
    }
}




calculator
// Calculator.java
class Calculator {
    int add(int a, int b) { return a + b; }
    int sub(int a, int b) { return a - b; }
    int mul(int a, int b) { return a * b; }
    int div(int a, int b) { return a / b; }
}
// Main.java
public class Main {
    public static void main(String[] args) {
        Calculator c = new Calculator();
        System.out.println(c.add(10, 5));
        System.out.println(c.sub(10, 5));
        System.out.println(c.mul(10, 5));
        System.out.println(c.div(10, 5));
    }
}
