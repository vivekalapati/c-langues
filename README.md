using System;

class Program
{
    static void Main()
    {
        Console.Write("Enter student name: ");
        string name = Console.ReadLine();

        Console.Write("Enter marks in Java: ");
        int java = Convert.ToInt32(Console.ReadLine());

        Console.Write("Enter marks in SQL: ");
        int sql = Convert.ToInt32(Console.ReadLine());

        Console.Write("Enter marks in Python: ");
        int python = Convert.ToInt32(Console.ReadLine());

        int total = java + sql + python;
        double average = total / 3.0;

        Console.WriteLine("\nStudent Details");
        Console.WriteLine("Name: " + name);
        Console.WriteLine("Total Marks: " + total);
        Console.WriteLine("Average Marks: " + average);

        if (average >= 50)
        {
            Console.WriteLine("Result: Pass");
        }
        else
        {
            Console.WriteLine("Result: Fail");
        }
    }
}
