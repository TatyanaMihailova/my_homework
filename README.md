// Задайте значения M и N. Напишите программу, которая выведет все натуральные числа в промежутке от M до N. Использовать рекурсию, не использовать циклы. 

using System;

namespace RecursionExample
{
    classProgram
    {
        static void Main(string[] args)
        {
            // Задайте значения M и N
            int m =5;
            intn= 10;

            // Вызовите рекурсивную функцию для вывода чисел
            PrintNumbers(m, n);
        }

        static void PrintNumbers(int m, int n)
        {
            // Базовый случай:��сли m больше n, остановите рекурсию
            if (m > n)
            {
                return;
            }

            // Выведите текущее число m
            Console.WriteLine(m);

            // Рекурсивно вызовите функцию с m + 1
            PrintNumbers(m + 1, n);
        }
    }
}