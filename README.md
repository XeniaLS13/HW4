# Домашняя работа 4

## Задание 1
### Напишите программу, которая выводит массив из 8 элементов, заполненный нулями и единицами в случайном порядке. Самое левое число не равно 0. Данный массив есть двоичное представление десятичного числа [1, 0, 1, 1, 0, 1, 0, 0]. Реализовать перевод двоичного числа в десятичное

[Код](https://github.com/XeniaLS13/HW4/blob/main/Task1/Program.cs)

## Задание 2
### Напишите программу, которая принимает на вход число и выдаёт сумму цифр в числе.

452 -> 11

82 -> 10

9012 -> 12

[Код](https://github.com/XeniaLS13/HW4/blob/main/Task2/Program.cs)

## Задание 3 (из лекции)
### Каким образом адаптировать код упорядочивания массива от минимального элемента к максимальному элементу таким образом, чтобы упорядочивание проводилось в обратном порядке? 

Исходный код: 

void SelectionSort(int[] array)

{

    for(int i = 0; i < array.Length - 1; i++)

    {

        int minPosition = i;

        for(int j = i + 1; j < array.Length; j++)

        {
            if (array[j] < array[minPosition])

            {

                minPosition = j;

            }

        }

        int temporary = array[i];

        array[i] = array[minPosition];

        array[minPosition] = temporary;

    }
    
}

[Код](https://github.com/XeniaLS13/HW4/blob/main/Task3/Program.cs)