// Напишите программу вычисления функции Аккермана с помощью рекурсии. Даны два неотрицательных числа m и n.

using System;

class Program
{
    static int Ackermann(int m, int n)
    {
        if (m == 0)
        {
            return n + 1;
        }
        else if (n == 0)
        {
            return Ackermann(m - 1, 1);
        }
        else
        {
            return Ackermann(m - 1, Ackermann(m, n - 1));
        }
    }

    static void Main()
    {
        Console.Write("Введите неотрицательное число m: ");
        int m = Convert.ToInt32(Console.ReadLine());
        Console.Write("Введите неотрицательное число n: ");
        int n = Convert.ToInt32(Console.ReadLine());

        Console.WriteLine($"Результат функции Аккермана для A({m}, {n}) = " + Ackermann(m, n));
    }
}