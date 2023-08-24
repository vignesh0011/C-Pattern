# PATTERN
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
Otherwise use else to print the inner value
```val = val * (i - j + 1) / j```
### Step 7:
Print the program.
### Step 8:
End of the Program.
## Program:
```C#
using System;
public class Pascal
{
    public static void Main()
    {
        int r, c = 1, s, i, j;
        r = Convert.ToInt32(Console.ReadLine());
        for (i = 0; i < r; i++)
        {
            for (s = 1; s <= r - i; s++)
                Console.Write("  ");
            for (j = 0; j <= i; j++)
            {
                if (j == 0 || i == 0)
                    c = 1;
                else
                    c = c * (i - j + 1) / j;
                Console.Write("{0}   ", c);
            }
            Console.Write("\n");
        }}}     
```
## Output:
![image](https://github.com/vignesh0011/C-Pattern/assets/53014593/4cc668b1-4131-4f47-8643-70d8e0abc4b1)
## Result:
Hence, a C# program for a pascal's triangle is executed successfully.
