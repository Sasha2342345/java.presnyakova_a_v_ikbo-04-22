//1. Создать проект в IntelliJ IDEA
//2. Создать свой собственный Git репозитoрий
//3. Написать программу, в результате которой массив чисел создается с помощью инициализации (как в Си) вводится и считается в цикле сумма элементов целочисленного массива, а также 
//среднее арифметическое его элементов результат выводится на экран. Использовать цикл for.
//4. Написать программу, в результате которой массив чисел вводится пользователем с клавиатуры считается сумма элементов целочисленного массива с помощью циклов do while, while, 
//также необходимо найти максимальный и минимальный элемент в массиве, результат выводится на экран.
//5. Написать программу, в результате которой выводятся на экран аргументы командной строки в цикле for.
//6. Написать программу, в результате работы которой выводятся на экран первые 10 чисел гармонического ряда (форматировать вывод).
//7. Написать программу, которая с помощью метода класса, вычисляет факториал числа (использовать управляющую конструкцию цикла), проверить работу метода.
//8. Результаты выполнения практической работы залить через IDE в свой репозитoрий и продемонстрировать преподавателю.








package com;
import java.util.Scanner;
public class Main {

    public static void main(String[] args) {


        //задание 3
        /*
        // Ввод длины массива
        Scanner sc = new Scanner(System.in);
        System.out.print("Введите количество необходимых чисел: ");
        int length;
        length = sc.nextInt();

        // Заполнение массива
        int[] numbers = new int[length];
        for (int i = 0; i < length; i++) {
            Scanner number = new Scanner(System.in);
            System.out.print("Введите целое число: ");
            numbers[i] = number.nextInt();
        }

        // Сумма чисел в массиве
        int sum = 0;
        for (int i = 0; i < length; i++) {
            sum += numbers[i];
        }

        // Результат
        System.out.println("Сумма введенных чисел: " + sum);
        System.out.println("Среднее арифметическое введенных чисел: " + (sum/length));
        */


        //задание 4
        /*
        // Ввод длины массива
        Scanner sc = new Scanner(System.in);
        System.out.print("Введите количество необходимых чисел: ");
        int length;
        length = sc.nextInt();

        // Заполнение массива
        int[] numbers = new int[length];
        for (int i = 0; i < length; i++) {
            Scanner number = new Scanner(System.in);
            System.out.print("Введите целое число: ");
            numbers[i] = number.nextInt();
        }

        // Сумма с помощью do while
        int sum1 = 0; int k = 0;
        do {
            sum1 += numbers[k];
            k++;
        } while (k < length);
        System.out.println("Сумма с помощью do while = " + sum1);

        // Сумма с помощью while
        int sum2 = 0; k = 0;
        while (k < length){
            sum2 += numbers[k];
            k++;
        }
        System.out.println("Сумма с помощью while = " + sum2);

        // Поиск минимума и максимума
        int max = 0; int min = 9999;
        for (int i = 0; i < length; i++) {
            if (max < numbers[i])
                max = numbers[i];
            else
                min = numbers[i];
        }
        System.out.println("Минимальное значение = " + min);
        System.out.println(("Максимальное значение = " + max));
        */






        //задание 5
        /*
        for (int i = 0; i < args.lenght; i++) {
            System.out.println(args[i]);
        }
        */



        //задание 6
        /*
        System.out.println("Первые 10 чисел гармонического ряда:");

        for (int i = 1; i <= 10; i++) {
            double harmonicNumber = 1.0 / i;
            System.out.printf("1/%d = %.2f\n", i, harmonicNumber);

        }
        */





        //задание 7
    
      System.out.println(calculateFactorial(4));
    }
  
    static int calculateFactorial(int n){
      int result = 1;
      for (int i = 1; i <=n; i ++){
          result = result*i;
      }
      return result;
      }
}




