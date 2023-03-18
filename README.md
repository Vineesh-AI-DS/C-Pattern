# Pattern

## Aim:

To write a C# program for a pascal's triangle

## Equipment Required:

Microsoft Visual Studio 2022 (or Lower) or Any other C# compiler

## Algorithm:

### Step 1:
Create a new Class named pascal.

### Step 2:
Declare two variables of int data type one to store the input from user for no.of rows snd another the value for printing.

### Step 3:
Get the number of rows from the user.

### Step 4:
Using for loop print the rows and columns and space.

### Step 5:
Check the first and last rows of the triange is 1 using if condition.

### Step 6:
Otherwise use else to print the inner value val = val * (i - j + 1) / j

### Step 7:
Print the program.

### Step 8:
End of the Program.

## Program:
```
Developed By: Vineesh.M
Register Number : 212221230122
```
```cs
using System;
namespace Pattern
{
    public class pascaltraingle
    {
        public static void Main(string[] args)
        {
            int row, c = 1;

            Console.Write("Enter rows: ");
            row = Convert.ToInt32(Console.ReadLine());

            for (int i = 0; i < row; i++)
            {
                for (int j = 1; j <= row - i; j++)
                    Console.Write(" ");
                for (int j = 0; j <= i; j++)
                {
                    if (j == 0 || i == 0)
                        c = 1;
                    else
                        c = c * (i - j + 1) / j;
                    Console.Write("{0} ", c);
                }
                Console.WriteLine();
            }
        }
    }
}
```

## Output:

![patt](https://user-images.githubusercontent.com/93427254/226119117-853fbcc0-f2bb-4b55-b5f8-710160f307e8.png)

## Result:
Hence, a C# program for a pascal's triangle is executed successfully.
