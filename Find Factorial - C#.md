This C# program calculates the factorial of a given integer. The factorial of a non-negative integer n (denoted as n!) is the product of all positive integers from 1 to n. This code snippet demonstrates how to compute the factorial using an iterative approach.



```Csharp

using System;

public class HelloWorld
{
    int res = 1;
    int inival = 1;

    // Method to find the factorial of a number
    public int FindFactorial(int x)
    {
        // Iteratively calculate factorial
        while (inival <= x)
        {
            res *= inival;
            inival++;
        }
        return res;
    }

    public static void Main(string[] args)
    {
        HelloWorld hw = new HelloWorld();
        // Example usage: Find factorial of 5
        Console.WriteLine(hw.FindFactorial(5)); // Output: 120
    }
}
