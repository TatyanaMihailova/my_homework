// Задайте значения M и N. Напишите программу, которая выведет все натуральные числа в промежутке от M до N. Использовать рекурсию, не использовать циклы.
void NumbersInTheRangeFromMton(int num1, int num2)
{
    if (num1 > num2) return;
        Console.Write($"{num1} ");
        void NumbersInTheRangeFromMton(int num1+1, int num2);
    }

    Console.WriteLine("Введите первое число");
    int M = Convert.ToInt32(Console.ReadLine());

    Console.WriteLine("Введите второе число");
    int N = Convert.ToInt32(Console.ReadLine());

    NumbersInTheRangeFromMton(M, N);
}# TatyanaMihailova
