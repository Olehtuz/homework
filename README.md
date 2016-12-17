
	1. Создайте калькулятор, который выполняет, базовые арифметические операции:
     - умножение;
     - деление;
     - сложение;
     - вычитание;
     - остаток от деления (%);
     - нахождение модуля числа (можно использовать Math.abs - стандартный класс из rt.jar, или написать свою функцию)
       входные данные здесь можно представить как:
         String operation = "addition";
         int firstOperand = 15;
         int secondOperand = 12;
         
	2. Добавить к калькулятору возможность ввода операции и чисел из консоли.
     В начале выводите сообщение "Введите операцию:", дальше пользователь вводит операцию,
     далее "Введите первое число:" - вводит,
     "Введите второе число: " - пользователь вводит.
        Пример ввода чисел и строки:
        Scanner scanner = new Scanner(System.in);
        int op1 = scanner.nextInt();
        int op2 = scanner.nextInt();
        String operation = scanner.next();
        Обратите внимание на то, что нужно импортировать класс Scanner из rt.jar (import java.util.Scanner;)
	
  	3. Тот же калькулятор, только операция и числа вводятся как параметры из командной строки.
	Пример запуска:
	java -cp result.jar com.hillel.MyMainClass 5 8 addition
	
 	4. Задача "Чаевые":
     входные данные: сумма, которую вы должны заплатить и уровень сервиса
     в зависимости от уровня сервиса посчитайте количество денег, которое вы должны оставить:
      - terrible (0%)
      - poor (5%)
      - good (10%)
      - great (15%)
      - excellent (20%)