# __Команды Java__

## __Создание класса programm__

Для создания класса достаточно использовать снипит class и выбрать его и программа сразу же скомпилирует класс:

    public class program {
        
    }

## __Точка входа__
Точка входа с корой компилятор начинает выполнение инструкций это метод main:

    public static void main(String[] args) {

    }

## __Вывод результата__

Для вывода результата в консоль используйте следующий скрипт:

    System.out.prontln("Hello World!");

## __Создание переменной__

Для создания переменной как и в С# нам необходимо для начала определить <тип_переменной> потом <имя_переменной> и в Java обязательно переменной необходимо присвоить <начально_значение> иначе компилятор выдаст ошибку:

___Пример:___

    int number = 10;
    double numberDouble = 8.34;
    float numberFloat = 1.24f;
    string s = "Hello World!!!";
    boolean flag = true;

## __Кассы обёртка__
Данные классы позволяют нам работать с переменными с помощью встроенной бибилиотеки инструкций

    int     : Integer
    shor    : Short
    long    : Long
    byte    : Byte
    float   : Float
    double  : Double
    char    : Character
    boolean : Boolean

___Пример:___

    int i = 123;
    System.out.println(Integer.MAX_VALUE);

Integer.MAX_VALUE; выводит максимаольно допустимое значение которое может принять переменная "int"
## __Массивы__

Примеры написания массивов чисел:

    int[] array = new int[10];
    int[] array1 = new int[] { 1, 10, 2, 8}
    array[3] = 13;
    System.out.println(array.length);

Пример написания многомерных массивов:

    int[] array[] = new int[3][5];

    int[][] array1 = new int[3][5];// массив массивов

## __Преобразовани__


## __Получение данных с терминала__

Для получения данных с терминала необходимо импортировать библиотеку _Java.util.Scanner_

    import java.util.Scanner;

    public class programm {
        public static void main(String[] args) {
            Scanner iScanner = new Scanner(System.in);
            System.out.printf("name: "); // можно println
            String name = iScanner.nextLine();
            System.out.println("Привет, %s!", name);
            iScanner.close();
        }
    }


__Пример получения значени типа int или double__
  
    import java.util.Scanner;

    public class programm {
        public static void main(String[] args) {
            Scanner iScanner = new Scanner(System.in);
            System.out.printf("int number: "); // можно println
            int number = iScanner.nextInt();
            System.out.println("double number: ");
            duble number = iScanner.nextDouble();
            iScanner.close();
        }
    }