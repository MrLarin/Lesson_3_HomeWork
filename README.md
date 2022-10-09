# Lesson_3_HomeWork

## Задача 19. На входе дано пятизначное число. НЕобходимо вывести является ли оно полиндромным.
```
int a = 0;
Console.Write($"Введите пятизначное число: ");
int.TryParse(Console.ReadLine()!, out a);
Console.Write(a);
if (a / 10000 == a % 10 && a / 1000 % 10 == a / 10 % 10)
    Console.Write(" - Число является полиндромным");
else
    Console.Write(" - Число НЕ является полиндромным");
```

## Задача 21. Напишите программу, принимает на вход координаты двух точек и находит расстояние между ними в 3D пространстве.(Я просто хотел через рандом заполнить и и использовать методы функции)
```
void FillArray(int[] Coll)
{
    int length = Coll.Length;
    int i = 0;
    while (i < length)
    {
        Coll[i] = new Random().Next(1, 100);
        i++;
    }
}

void PrintArray(int[] Collection)
{
    int count = Collection.Length;
    int j = 0;
    while (j < count)
    {
        Console.Write($"{Collection[j]}, ");
        j++;
    }
}

int[] Array1 = new int[3];
FillArray(Array1);
PrintArray(Array1);
Console.WriteLine();
int[] Array2 = new int[3];
FillArray(Array2);
PrintArray(Array2);
Console.WriteLine();

int A = (int)Math.Pow((Array1[0] - Array2[0]), 2);
Console.WriteLine(A);
int B = (int)Math.Pow((Array1[1] - Array2[1]), 2);
Console.WriteLine(B);
int C = (int)Math.Pow((Array1[2] - Array2[2]), 2);
Console.WriteLine(C);
double Z;
Console.Write($"Расстояние между точками -  {Z = Math.Sqrt(A + B + C)}");
```

## Задача 23. Написать программу, котораяна вход принимает число (N), и выыдает таблицу кубов чисел от 1 до N. 3-> 1, 8, 27. 5-> 1, 8, 27, 64, 125.
```
int N;
Console.Write($"Введите число: ");
int.TryParse(Console.ReadLine()!, out N);
Console.Write(N);
Console.WriteLine();
for (int i = 1; i <= N; i++)
    Console.Write($"{i * i * i} ");
```
