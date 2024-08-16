This code calculates the Fibonacci number at a given position using an iterative approach. The Fibonacci sequence is defined by:


```Csharp

using System;

public class FibonacciCalculator
{
    // Method to find the Fibonacci number at position 'n'
    public int FindFibonacci(int n)
    {
        if (n <= 1) return n;
        
        int a = 0, b = 1;
        for (int i = 2; i <= n; i++)
        {
            int temp = a + b;
            a = b;
            b = temp;
        }
        return b;
    }

    public static void Main(string[] args)
    {
        FibonacciCalculator calc = new FibonacciCalculator();
        // Example usage: Find Fibonacci number at position 5
        Console.WriteLine(calc.FindFibonacci(5)); // Output: 5
    }
}
