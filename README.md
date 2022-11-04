# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step 1:
Create a function for reversing.

### Step 2:
Get the number from the user.

### Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step 4:
Recusively call this function to get the reversed number.

### Step 5:
Print the reversed number.

## Program:
```
using System;
namespace Som
{
    class Program
    {
        int remainder = 0, rev = 0;
        public int reverse(int n)
        {
            remainder = n % 10;
            if (remainder == 0) return rev;
            else
            {
                rev = rev * 10 + remainder;
                return reverse(n / 10);
            }
        }
        static void Main(string[]args)
        {
            int n;
            Console.WriteLine("Enter numbers to be Reversed:");
            n =Convert.ToInt32(Console.ReadLine());

            Program p1 = new Program();
            Console.WriteLine("Reversed Numbers are:" + p1.reverse(n));
        }
    }
}
```

## Output:
![rev](https://user-images.githubusercontent.com/93434149/199885983-e0b5a066-a457-493e-979e-41154599cbc2.jpg)


## Result:
Thus to write a C# program to reverse a number using recursive function is successfully completed.

