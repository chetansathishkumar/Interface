# Interface

## Aim:
  To write a C# program using interface concept

## Algorithm:
## Step 1:
Create an interface.

## Step 2:
Create a child class.

## Step 3:
Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

## Step 4:
Create those 2 functions in the child class and perform respective operation.

## Step 5:
Use while loop and and switch case to Get the choice from the user whether to perform withdrawal or deposit operation.

## Step 6:
After performing the functions display the remaining balance of the user.

## Program:
```
using System;
public interface Bank
{
    public void deposit(int amount);
    public void withdrawal(int amount);
}
public class Example : Bank
{
    int balance = 5000;
    public void deposit(int amount)
    {
        balance += amount;
        Console.WriteLine(balance);
    }
    public void withdrawal(int amount)
    {
        balance -= amount;
        Console.WriteLine(balance);
    }
    public class Bank
    {
        public static void Main()
        {
            Example obj = new Example();
            Console.WriteLine("1. Deposit\n2. Withdrawal");
            int ch = Convert.ToInt32(Console.ReadLine());
            if (ch == 1)
            {
                int amount = Convert.ToInt32(Console.ReadLine());
                obj.deposit(amount);
            }
            else
            {
                int amount = Convert.ToInt32(Console.ReadLine());
                obj.withdrawal(amount);
            }
        }
    }

}
```

## Output:

![image](https://user-images.githubusercontent.com/75260837/203898353-375b29e5-558a-46f0-989a-447619a723f4.png)

## Result:
Thus the C# program using interface concept has been implemented successfully
