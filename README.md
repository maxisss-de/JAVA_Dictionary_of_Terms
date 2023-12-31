Словарь терминов. Основы Java
==================================

Обратите внимание, что слова расположены в алфавитном порядке. Для быстрого перехода к нужному термину используйте команду “Поиск в документе” (Ctrl+F).


D
=============
 
### Do while / цикл “делать до тех пор пока” / цикл с постусловием

Do while - оператор **цикла**, который повторяет блок кода, пока заданное условие является верным (его еще называют цикл "делать до тех пор пока"). Используется, когда заранее неизвестно, сколько раз нужно что-то сделать, но при этом известны условия прекращения цикла (и эти условия должны проверяться строго после того, как выполнится тело цикла). Цикл do while проверяет условия в конце тела цикла, поэтому называется циклом с постусловием. Цикл do…while удобно использовать, когда некоторое действие в программе нужно выполнить по крайней мере единожды, но при некоторых условиях придётся повторять его многократно. Цикл имеет следующий синтаксис:

    do {
        инструкция;
        ...
        инструкция; / инструкции внутри фигурных скобок составляют тело цикла
    } while (условие); 

**Пример:**  выведем на экран числа от 1 до 5

    int i = 0;
    do {
       i = i + 1;
       System.out.print(i);
    } while(i < 5);

*Подробнее в лекции:*

1. лекция “4 Циклы” из “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “1.3 Условные операторы и циклы” из “Блок 1. Основы Java”.
 
 

F
=================

### For / цикл со счетчиком

For - оператор **цикла**, который  выполняет последовательность кода (тела цикла) столько раз, сколько определено в его переменной счетчика, и называется циклом “со счетчиком”. Такой цикл хорошо подходит, когда заранее точно известно, сколько раз нужно повторить одно и то же действие (или набор действий). Цикл имеет следующий синтаксис:

    for (начало; условие; шаг) {
      // ... тело цикла ...
    }

*Начало* - это объявление и инициализация переменной, которая является счетчиком выполненных итераций цикла. *Условие* - это выражение, выполняющееся на каждой итерации цикла (если выражение истинно, цикл выполняется). *Шаг* - это выражение, которое выполняется в самом конце цикла и используется для обновления (увеличения) значения переменной счётчика.

**Пример:** выведем на экран числа от 1 до 5

    for (int i = 1; i < 6; i++) {
      System.out.print(i);
    }
    // Результатом будет: 1 2 3 4 5

*Подробнее в лекции:*

1. лекция “4 Циклы” из “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “1.3 Условные операторы и циклы” из “Блок 1. Основы Java”.
 
 
 
### Foreach 

Foreach  является оператором **цикла**,  разновидностью цикла **for**. Используется для перебора элементов **массива** или коллекции. Его сигнатура не включает присвоение начального значения счетчика и его последующий инкремент (увеличение).

**Пример:** для того чтобы вывести слово Борщ, перебрав все элементы массива, достаточно использовать цикл с перебором элементов этого массива.

    char[] borsh = {'Б','о', 'р', 'щ'};
    foreach(char letter : borsh) {
        System.out.print(letter);
    }

*Подробнее в лекции:*
лекция “1.3 Условные операторы и циклы” из “Блок 1. Основы Java”.
 
 
 
J
===================

### Java

Java — объектно-ориентированный язык программирования высокого уровня, был разработан Джеймсом Гослингом и компанией Sun Microsystems (впоследствии поглощенной компанией Oracle). Первая версия языка была выпущена 21 января 1996 г. С сентября 2018 года актуальной версией является Java 11. 

Java превратилась из просто универсального языка в целую платформу и экосистему, которая объединяет различные технологии, используемые для целого ряда задач: от создания десктопных приложений (программы, которые запускаются с рабочего стола компьютера) до написания крупных веб-порталов.

Ключевой особенностью языка Java является то, что его код сначала транслируется в специальный **байт-код**, независимый от операционной среды, а затем этот байт-код выполняется виртуальной машиной **JVM (Java Virtual Machine)**, которая устанавливается на любую операционную среду.

[*Подробнее >*](https://ru.wikipedia.org/wiki/Java)

[*Подробнее про высокоуровневое программирование >*](https://ru.wikipedia.org/wiki/%D0%92%D1%8B%D1%81%D0%BE%D0%BA%D0%BE%D1%83%D1%80%D0%BE%D0%B2%D0%BD%D0%B5%D0%B2%D1%8B%D0%B9_%D1%8F%D0%B7%D1%8B%D0%BA_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F)

[*Подробнее про объектно-ориентированное программирование >*](https://ru.wikipedia.org/wiki/%D0%9E%D0%B1%D1%8A%D0%B5%D0%BA%D1%82%D0%BD%D0%BE-%D0%BE%D1%80%D0%B8%D0%B5%D0%BD%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5)
 
 
 
### Java-байт-код / байт-код Java / байт-код / bytecode

Байт-код Java — набор команд, в которые преобразуется (компилируется) программа, написанная на языке **java**. Эти команды затем исполняются **виртуальной машиной Java (JVM)**. Каждая такая команда занимает в памяти 1 байт. Перед тем как запустить любую программу на Java, нужно обязательно компилировать написанный код в команды, которые будут выполняться на JVM. Для программирования на языке Java знание особенностей байт-кода не обязательно.

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%91%D0%B0%D0%B9%D1%82-%D0%BA%D0%BE%D0%B4_Java)
 
 
 
### Javac 

Javac - специальная программа-компилятор (входит в **Java Development Kit**), которую нужно использовать для преобразования программы, написанной на языке **java**, в **байт-код**, исполняемый **виртуальной машиной Java**. Компиляция с помощью javac осуществляется либо в **консоли** (в режиме “командной строки”), либо через **IDE**.

[*Подробнее >*](https://ru.wikipedia.org/wiki/Javac)



### JDK / Java Development Kit  

JDK  - комплект средств (сервисов) разработчика. Содержит необходимые библиотеки и подпрограммы для запуска, компиляции и отладки программ на языке java. Используется при разработке программ на языке java. Разрабатывается компанией Oracle и open-source community. Все современные **интегрированные среды разработки (IDE)** для java, такие как IDEA, Eclipse, NetBeans, Android Studio, используют JDK.

**Пример:** 

1) Java SE Development Kit 8 - Downloads Инструкция по установке: https://github.com/netology-code/guides/tree/master/intellij_idea
2) https://openjdk.java.net/

[*Подробнее >*](https://ru.wikipedia.org/wiki/Java_Development_Kit) 


 
### JRE / Java Runtime Environment / Среда выполнения для Java

JRE - это среда (программа), необходимая для запуска и выполнения программ, написанных на **java**. Она содержит только **виртуальную машину Java** для запуска программ и базовые библиотеки java-классов. В ней нет **компилятора** и средств для разработки. JRE полезна, если мы хотим только запустить готовую (уже скомпилированную) в **байт-код** программу.

**Пример:** https://www.java.com/ru/download/

[*Подробнее >*](https://ru.wikipedia.org/wiki/Java_Runtime_Environment)


 
### JVM / Java Virtual Machine / Виртуальная машина Java

JVM - это среда выполнения (программа для выполнения) программ, написанных на Java и преобразованных (скомпилированных) в байт-код.
Ключевой особенностью языка Java является то, что его код сначала транслируется в специальный байт-код, независимый от операционной среды. А затем этот байт-код выполняется виртуальной машиной JVM (Java Virtual Machine), которая устанавливается на любую операционную среду. Эта особенность Java позволяет писать программы для разных операционных систем и для разных устройств. Т.е. один и тот же код будет работать на разных платформах (Windows, Linux, Mac OS и т.д.) без изменений, понадобится только своя версия виртуальной машины JVM.

[*Подробнее >*](https://ru.wikipedia.org/wiki/Java_Virtual_Machine)



I
===================

### IDE / Integrated Development Environment / Интегрированная среда разработки

IDE — это единая среда разработки для создания приложения. Обычно IDE включает в себя: текстовый редактор, транслятор (компилятор и/или интерпретатор), средства автоматизации сборки, отладчик. Иногда содержит также средства для интеграции с системами управления версиями и другие инструменты.

**Пример:** 
Eclipse, NetBeans, IntelliJ IDEA.  Инструкция по установке Intellij Idea: https://github.com/netology-code/guides/tree/master/intellij_idea

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%98%D0%BD%D1%82%D0%B5%D0%B3%D1%80%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D0%B0%D1%8F_%D1%81%D1%80%D0%B5%D0%B4%D0%B0_%D1%80%D0%B0%D0%B7%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B8)


 
### If / Условный оператор if

If — условный **оператор** (самый часто используемый). Он проверяет условие, указанное в качестве аргумента: `if (условие)`. Если результат вычисления условия верен, то программа продолжит выполнение кода, написанного внутри блока `{ код }`. Если результат не верен, то программа пропустит этот блок. Если нужно проверить несколько условий, к оператору `if` добавляется оператор `else` (иначе) и блок кода `{ код }`. Для проверки более чем одного условия операторы `if else` размещаются друг за другом.

**Пример:** 

1.Если температура чайника достигла 100 градусов, выполни код (выключи его): 

     if (temperatureTeapot == 100) {
         // Код сработает, только если переменная temperatureTeapot = 100;
     }

2.Если температура чайника достигла 100 градусов, выполни код (выключи его). Если нет, то продолжай кипятить воду в нем.

     if (temperatureTeapot == 100) {
         // Код в этом блоке сработает, только если переменная temperatureTeapot = 100;
     } else {
         // Код в этом блоке сработает, только если переменная temperatureTeapot не равна 1;
     }

*Подробнее в лекции:*
лекция “1.3 Условные операторы и циклы” из “Блок 1. Основы Java”.
 


 S
 =======================
 
### Switch / Условный оператор switch

Switch -  условный **оператор**, который в качестве аргумента принимает переменную и сравнивает ее значение в инструкциях оператора `case`. Дополнительно оператор `switch` имеет инструкцию `default`, определяющую вариант по умолчанию (срабатывает в случае, если ни один из вариантов оператора `case` не совпал).

**Пример:** в зависимости от температуры холодильника включите или отключите компрессор охлаждения в нем.

    switch (refrigeratorTemperature) {
        case 0:
            // Код в этом блоке сработает, только если переменная refrigeratorTemperature = 0;
            break;
        case -20:
            // Код в этом блоке сработает, только если переменная refrigeratorTemperature = -20
            break;
        default:
            // Код в этом блоке сработает, если ни одно условие выше не оказалось верным;
    }

*Подробнее в лекции:*
 лекция “1.3 Условные операторы и циклы” из “Блок 1. Основы Java”.
 


W
=======================
 
### While / Цикл "пока" / Цикл "до тех пор пока” /  Цикл с предусловием

While - оператор **цикла**, который повторяет блок кода, пока заданное условие является верным (его еще называют цикл "пока" или "до тех пор пока”). Используется, когда заранее неизвестно, сколько раз нужно что-то сделать, но при этом известны условия прекращения цикла (и эти условия должны проверяться строго до того, как выполнится код внутри цикла). Цикл проверяет условие до выполнения тела цикла, поэтому цикл while называется циклом с предусловием. Цикл имеет следующий синтаксис:

    while (условие) {
        инструкция;
        ...
        инструкция;
        // инструкции внутри фигурных скобок составляют тело цикла
    }

**Пример:** выведем на экран числа от 1 до 5

    int i = 0;
    while (i < 5) {
        i = i + 1;
        System.out.println(i);

*Подробнее в лекции:*

1. лекция “4 Циклы” из “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “1.3 Условные операторы и циклы” из “Блок 1. Основы Java”.



А
===============
 
### Абстрактные классы 

Абстрактные классы в программировании позволяют создать механизм, который позволял бы описать общие свойства объектов, реализовать одинаковые для всех методы так, чтобы разработчик классов-наследников мог реализовывать только отличающиеся части. Абстрактный класс, как и обычный, содержит поля и методы, но нельзя создать экземпляр абстрактного класса. Также в отличие от обычного класса, абстрактный может содержать методы без реализации (абстрактные).

Абстрактные методы (могут быть только внутри абстрактного класса) не содержат реализации и обязательно должны быть переопределены в потомках.

**Пример:** создание абстрактного класса геометрических фигур (класс обобщает свойства различных фигур):

    abstract class Figure {
        private Color fillColor;
        public Color(Color fillColor) {
            this.fillColor = fillColor;
        }
        public Color getFillColor() { 
            return fillColor; 
        }
        public abstract double getPerimeter();
        public abstract double getArea();
    }

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%90%D0%B1%D1%81%D1%82%D1%80%D0%B0%D0%BA%D1%82%D0%BD%D1%8B%D0%B9_%D0%BA%D0%BB%D0%B0%D1%81%D1%81)

*Подробнее в лекции:*
лекция “3.4. Основы ООП - абстракции и интерфейсы” из “Блок 3. Основы ООП”



Д
===================
 
### Двумерный массив 

Двумерный массив - это **массив**, в котором для определения местоположения элемента в массиве нужно указать значения двух **индексов**. Двумерный массив ассоциируется с таблицей. Если количество столбцов и строк массива (таблицы) одинаковое, то массив еще называют **матрицей**. 

При объявлении двумерного массива указываем тип, размеры и имя. Массив можно создать тремя способами:

1) `тип имя_переменной[][] = new тип[размер][размер]`; 
2) `тип[][] имя_переменной = new тип[размер][размер]`; 
3) `тип[] имя_переменной[] = new тип[размер][размер]`;

*тип* – базовый тип элементов массива; *размер* – число элементов массива. Элементы массива могут быть любого типа, допустимого в языке Java. Важный момент - размер созданного массива нельзя изменить. 

**Пример:** объявим двумерный строковый массив с именем products (размер массива 2x4) и заполним значениями: 

    String products[][] = new String[2][4];
        products[0][0] = "Хлеб";
        products[0][1] = "ООО ГРУП";
        products[0][2] = "5 дней";
        products[0][3] = "мука";
    
        products[1][0] = "Сметана";
        products[1][1] = "ИП Про";
        products[1][2] = "10 дней";
        products[1][3] = "молоко";
 
*Подробнее в лекции:*
лекция “2.2 Массивы многомерные” из “Блок 2. InMemory хранение данных — массивы”.
 
 

И
=================
 
### Индекс 

В программировании одно из значений индекса - это позиция элемента в **массиве** (начинается индекс с нуля). Индекс указывается в квадратных скобках `[ ]` после имени массива.

**Пример:**  создание массива с тремя целочисленными элементами и присвоение значения каждому из элементов:

    int[] array1 = new int[3]; 
            array1[0] = 5;
            array1[1] = 17;
            array1[2] = 350;
 
*Подробнее в лекции:*
1. лекция “6 Массивы” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “2.1 Массивы одномерные” из “Блок 2. InMemory хранение данных — массивы”.


 
### Инициализация переменной

Инициализация **переменной** означает присвоение начального значения переменной. Инициализация может происходить как одновременно с объявлением переменной, так и после.

**Пример:**

    int number = 5 ; //создаем переменную с именем number с численным типом int и присваиваем ей значение 5 
 


### Интерфейс (interface) объекта 

Интерфейс представляет собой внешнее описание **объекта** и описывается атрибутами и методами объекта, которые доступны для использования другими объектами. Конкретный интерфейс описывает поведение (набор методов) объекта, реализующего данный интерфейс (в отличие от класса, который может еще и хранить состояние). Реализация конкретного интерфейса некоторым классом говорит о том, что объекты этого класса можно использовать определенным образом. Это позволяет работать одинаково с объектами разных классов.

В отличие от **абстрактных классов** интерфейсы описывают только поведение (методы), могут быть реализованы на абсолютно разных классах,при этом класс может реализовывать несколько интерфейсов. Механизм использования интерфейса решает проблему запрета (нежелательности) множественного наследования классов в объектно-ориентированном  программировании.

**Пример:** мы хотим добавить нашим объектам-фигурам возможность изменять масштаб:

    public interface Scalable {
        public void scale(int factor);
    }

Теперь любой класс, реализующий интерфейс Scalable, обязан иметь метод scale.

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%98%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81_(%D0%BE%D0%B1%D1%8A%D0%B5%D0%BA%D1%82%D0%BD%D0%BE-%D0%BE%D1%80%D0%B8%D0%B5%D0%BD%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекции:*
лекция “3.4. Основы ООП - абстракции и интерфейсы” из “Блок 3. Основы ООП”
 
 

К
==================
 
### Класс 

Класс - это специальная структура, c помощью которой описываются будущие **объекты** в java. Чтобы описать класс нужно: 
1) создать файл с именем класса и расширением java; 
2) внутри этого файла добавить специальный оператор `class` и "Имя файла". 

Класс может содержать в себе **поля** (характеристики объекта, или переменные внутри класса) и **методы** (функции, которые может выполнять объект). Названия классов в Java пишутся с большой буквы, а названия объектов — с маленькой.

**Пример:**  создание класса “музыкальная студия” с полями (название; владелец; год основания; количество выпущенных треков) и двумя методами (увеличения количества сделанных студией записей и смены названия студии на случай ребрендинга):

    class RecordStudio {
        String label;
        String owner;
        int foundationYear;
        int records;
    
        void makeNewRecord() {
            records++;
        }
    
        void setLabel(String newLabel) {
            label = newlabel;
        }
    }


[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9A%D0%BB%D0%B0%D1%81%D1%81_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекции:*
1. лекция “5. Классы и объекты” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “3.1 Структура класса” из “Блок 3. Основы ООП”
 
 
### Компилятор

Компилятор - это программа (утилита), преобразующая файлы с исходным кодом (в языке java - это файлы с расширением java) в файлы, исполняемые компьютером (операционной системой). В экосистеме Java под компилятором понимается утилита, преобразующая программу, написанную программистом на java, в **байт-код**, исполняемый **виртуальной машиной Java**.   

**Пример:** **javac** - программа-компилятор, входящая в пакет **JDK**.

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BC%D0%BF%D0%B8%D0%BB%D1%8F%D1%82%D0%BE%D1%80)
 
 
### Компиляция

В программировании на **Java** под компиляцией понимается преобразование кода, написанного программистом на языке Java, в код, который понятен **виртуальной машине Java** (т.е. **байт-код**).

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BC%D0%BF%D0%B8%D0%BB%D1%8F%D1%82%D0%BE%D1%80)

 
### Константа

Константа - это имя, с которым связано некоторое постоянное значение (в отличие от **переменной** это значение единожды задаётся и потом уже не изменяется). Условно можно сказать, константы позволяют задать такие “переменные”, которым можно присвоить значение только один раз и потом это значение нельзя изменить. Константа объявляется также как и переменная, только вначале идет ключевое слово final. Как правило, константы имеют имена в верхнем регистре.

**Пример:** 

    final int LIMIT_IN_ATM = 5;

*Подробнее в лекциях:*
лекция “2 Переменные и типы данных” из “Блок 0. Введение в Java (Basic Java BJAVA)”.
 
 
### Консоль / терминал

В широком смысле консоль - это совокупность устройств (в том числе устройств ввода-вывода), обеспечивающая взаимодействие человека-оператора с компьютером. В современной лексике программирования под консолью понимается специальное “окно” для вывода системных сообщений и выполнения команд (другое название - интерфейс командной строки).  Часто используется как синоним понятия **“терминал”**.

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%98%D0%BD%D1%82%D0%B5%D1%80%D1%84%D0%B5%D0%B9%D1%81_%D0%BA%D0%BE%D0%BC%D0%B0%D0%BD%D0%B4%D0%BD%D0%BE%D0%B9_%D1%81%D1%82%D1%80%D0%BE%D0%BA%D0%B8)

 
### Конструктор класса / конструктор

Конструктор - это специальный **метод** **класса**, который ничего не возвращает, но описывает то, каким образом должен быть собран/инициализирован новый **объект** (экземпляр класса), например, какие должны быть значения **полей** у только что созданного объекта. Без вызова конструктора невозможно создать экземпляр данного класса. Конструкторы выполняют инициализацию объекта, то есть создание нового экземпляра класса, подставляя значения из аргументов конструктора. Конструкторов у класса может быть сколько угодно.Если в классе не определено ни одного конструктора, то для этого класса компилятором автоматически создается конструктор без параметров (т.е. все поля, если они не примитивные значения, примут значения `null`). 

Конструкторы должны иметь тоже имя, что и класс. Чтобы внутри метода отличить параметр конструктора от поля, если они имеют одинаковые наименования, используется this - ссылка на объект.

**Пример:** создание класса с описанием клиента и двумя конструкторами:

    public class Client {
        String name; // имя
        String surname; // фамилия
        String dateOfBirth; // дата рождения
        String passportId; // номер паспорта
        String PIN; // PIN-код для карты
    
        //конструктор класса с двумя параметрами
        Client (String name, String surname) {
            this.name = name;
            this.surname = surname;
        }
 
        //конструктор класса с тремя параметрами
        Client (String name, String surname, String passportId) {
            this.name = name;
            this.surname = surname;
            this.passportId = passportId;
        }
        ...   //программный код с описанием методов класса
    }

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D0%BE%D1%80_(%D0%BE%D0%B1%D1%8A%D0%B5%D0%BA%D1%82%D0%BD%D0%BE-%D0%BE%D1%80%D0%B8%D0%B5%D0%BD%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекции:*
1. лекция “5. Классы и объекты” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “3.1 Структура класса” из “Блок 3. Основы ООП”
 

М
====================
 
### Массив

В программировании массив – это ссылочный тип данных, представляющий собой набор элементов (переменных) одного типа. Элементы массива могут быть любого типа, допустимого в языке Java. Для объявление массива надо указать тип, размер и имя. Массив можно создать двумя способами:
1) `тип имя_переменной[] = new тип[размер]`;
2) `тип[] имя_переменной = new тип[размер]`;

*Тип* – базовый тип элементов массива; *размер* – число элементов массива (выделение памяти для элементов). Элементы массива могут быть любого типа, допустимого в языке Java.

**Пример:** Предположим, у нас есть список цен на товары, определим массив типа int и дадим размер массиву (например у нас список из 5 цен):

    int[] prices = new int [5];

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9C%D0%B0%D1%81%D1%81%D0%B8%D0%B2_(%D1%82%D0%B8%D0%BF_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85))

*Подробнее в лекции:*
1. лекция “6 Массивы” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “2.1 Массивы одномерные” из “Блок 2. InMemory хранение данных — массивы”.
 
 
### Матрица

Матрица - это **двумерный массив**, в котором количество столбцов и строк массива (таблицы) одинаковое.

*Подробнее в лекции:*
 лекция “2.2 Массивы многомерные” из “Блок 2. InMemory хранение данных — массивы”.
 
 
### Методы

Методы - это “действия” (функции), которые может выполнять **объект**. Методы существуют в виде процедур и функций, которые должны находиться в описании **класса**. Методы предоставляют интерфейс, при помощи которого осуществляется доступ к данным объекта некоторого класса. С практической точки зрения методы нужны для разделения программного кода на логические части, они позволяют быстрей читать, дорабатывать и документировать код.

Для того чтобы описать метод, нужно объявить:
- *тип возвращаемого значения* (или ключевое слово `void`, которое “говорит”, что метод ничего не возвращает);
- *имя метода*;
- в круглых скобках передаются *входные параметры метода* (в случае, если их нет, в скобках пусто);
- *тело метода* описывается так же как и класс в фигурных скобках `{...}`.

**Пример:** в классе `RecordStudio` описан метод `makeNewRecord`, который позволяет увеличить количество сделанных студией записей (количество записей хранится в поле `records`):

    class RecordStudio {
        String label;
        String owner;
        int foundationYear;
        int records;
    
        void makeNewRecord() {
            records++;
        }
    }

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%BE%D0%B4_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекции:*
1. лекция “5. Классы и объекты” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “3.1 Структура класса” из “Блок 3. Основы ООП”
 
 
### Многомерный массив

Многомерный массив - **массив**, в котором для определения местоположения элемента в массиве нужно указать значения трех и больше **индексов**. С многомерными массивами можно работать так же, как и с **двумерными**, но только учитывая количество индексов.

*Подробнее в лекции:* 
 лекция “2.2 Массивы многомерные” из “Блок 2. InMemory хранение данных — массивы”.
 
 
### Модификаторы доступа

Модификаторы доступа - это ключевые слова, которые пишутся перед названиями **переменных**, **методов** и даже **классов**.В Java используются следующие модификаторы доступа:
- `public`: публичный, общедоступный класс или член класса. Поля и методы, объявленные с модификатором public, видны другим классам из текущего пакета и из внешних пакетов.
- `private`: закрытый класс или член класса, противоположность модификатору public. Закрытый класс или член класса доступен только из кода в том же классе.
- `protected`: такой класс или член класса доступен из любого места в текущем классе или пакете или в классах-наследниках, даже если они находятся в других пакетах
- `static`: Если указать static перед методом класса, он также будет принадлежать создаваемому классу - это значит, что при вызове таких методов не требуется создание объекта.
- `default`: модификатор по умолчанию. Когда мы не пишем модификатора доступа, он по умолчанию имеет значение default. Такие поля или методы видны всем классам в текущем пакете.
 
*Подробнее в лекции:*
лекция “3.2 Модификаторы доступа, наследование” из “Блок 3. Основы ООП”


О
===================
 
### Обертки над примитивами / классы-обертки /  классы-оболочки

Класс-обертка - это аналог **ссылочного типа** для каждого **примитивного типа данных**. Другое название этого вида классов - классы-оболочки (wrappers). Такие классы нужны для расширения функционала примитивных типов, например, для преобразования строки в число. 

**Пример:** 

    примитивный тип - класс-обертка:
    short - Short, 
    byte - Byte, 
    int - Integer, 
    long - Long, 
    float - Float, 
    double - Double, 
    char - Character, 
    boolean - Boolean

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9E%D0%B1%D1%91%D1%80%D1%82%D0%BA%D0%B0_(%D1%82%D0%B8%D0%BF_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85))


### Объект

Объект в программировании — это сущность, способная сохранять свое состояние (информацию) и обеспечивающая набор операций (поведение) для проверки и изменения этого состояния. То есть простыми словами, все элементы, с которыми вы будете работать в программном коде, будут объектами. Объект — это модель реальной сущности в программной системе, потому что программные системы предназначены для моделирования реальных систем. Объекты создаются из **классов** с помощью **конструкторов**.Для того, чтобы создать новый объект из класса в java используется **оператор** new. Вызов **метода** на экземпляре класса происходит через символ точки ('.') по следующей схеме: `имяОбъекта.название метода (<параметры если есть>)`

**Пример:** создание объекта класса `RecordStudio` с одновременным заполнением полей этого класса (название, собственник, год основания, количество записей):

    RecordStudio captainRecords = new RecordStudio("Captain Records", "Unkown", 2010, 131235);

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9E%D0%B1%D1%8A%D0%B5%D0%BA%D1%82_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекции:*
1. лекция “5. Классы и объекты” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “3.1 Структура класса” из “Блок 3. Основы ООП”

 
### Оператор

Оператор - это некоторая команда в языке программирования (иногда оператор называют “инструкцией”). Оператор является наименьшей автономной часть языка программирования.

**Пример:** условный оператор **if**, оператор цикла **for**.
 
 
П
=====================
 
### Пакеты классов

Пакеты классов – это папки, в которых хранятся классы одного модуля программы. Пакеты - это простой способ хранения классов по категориям. Существуют пакеты уже готовых классов Java. Для использования классов определенного пакета в своей программе его нужно импортировать в программу командой `import` и указанием имени пакета классов. Имя пакета объявляется в самом начале исходного файла программы.

**Пример:***
- java.io - пакет классов для операций ввода-вывода; 
- java.sql -  пакет для использования соединений к базе данных. 

[*Подробнее >*](https://ru.wikipedia.org/wiki/Package_(Java))

*Подробнее в лекциях:*
лекция “1.2 Структура программы” из “Блок 1. Основы Java”.
 
 
### Переменная

В Java переменная — это имя, с которым связано некоторое значение. Можно провести аналогию с контейнером (коробкой), в котором может храниться значение для дальнейшего использования в программе. Т.е. можно сравнить переменную с коробкой, в которой хранится какой-то предмет (в случае с программированием данный предмет — это *значение переменной*). Коробка может иметь надпись (*имя переменной*). А также для разных видов вещей могут использоваться разные виды коробок (вид коробки — *тип переменной*). 

В java для создания (объявления) переменной используем команду, включающую тип переменной и имя переменной. В качестве типа переменной нужно выбрать один из уже существующих в языке java типов данных (примитивный или ссылочный). Имя переменной придумываем сами: обычно это существительное, которое пишется маленькими латинскими буквами .Если имя переменной состоит из двух слов, то пишется слитно и как бы “горбиками” как у верблюда.

**Пример:** 

    int number; //создаем переменную с именем number с численным типом int
    int amountOfBooks; //создаем переменную с именем amountOfBooks с численным типом int

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9F%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D0%B0%D1%8F_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекциях:*
лекция “2 Переменные и типы данных” из “Блок 0. Введение в Java (Basic Java BJAVA)”.
 
 
### Поля

Поля представляют собой **переменные**, которые нужны для хранения, изменения и использования значений внутри **класса**. При создании класса поля - это объявление характеристик **объекта**. В java для создания (объявления) поля (переменной) используем команду, включающую тип переменной и имя переменной.

**Пример:** создание класса “музыкальная студия” со следующими полями: название; владелец; год основания; количество выпущенных треков

    class RecordStudio {
        String name;
        String owner;
        int foundationYear;
        int records;
    }

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%9F%D0%BE%D0%BB%D0%B5_%D0%BA%D0%BB%D0%B0%D1%81%D1%81%D0%B0)

*Подробнее в лекции:*
1. лекция “5. Классы и объекты” из  “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция “3.1 Структура класса” из “Блок 3. Основы ООП”
 
 
### Примитивные типы данных / Primitive Data Types

Примитивные типы данных - это типы данных, которые предоставляются языком программирования как базовая встроенная единица языка. В языке java они бывают четырех видов: целочисленный, вещественный, символьный, булевый.

Таблица примитивных типов данных в языке Java:

Целочисленные:

1. byte (целые числа, 1 байт, -128 до 127)
2. short (целые числа, 2 байта, -32768 до 32767)
3. int (целые числа, 4 байта, -2147483648 до 2147483647)
4. long (целые числа, 8 байт, -9223372036854775808 до 9223372036854775807)

Вещественные:

5. float (вещественные числа, 4 байта, -3.4E+38 до 3,4E+38)
6. double (вещественные числа, 8 байт, -1.7E+308 до 1.7E+308)

Другие:

7. boolean (значение истина/ложь, 1 байт, true/false)
8. char (символ Unicode, 2 байта, 1 Unicode символ)
 
*Подробнее в лекциях:*
 лекция 1.4 Типы данных в Java: примитивы из Блок 1. Основы Java


С
======================
 
### Сигнатура метода

Сигнатура метода - это имя метода плюс параметры (причем порядок параметров имеет значение). 

**Пример:**  

    public static void main(String[] args).
 
 
### Ссылочные типы данных / Reference Types

Ссылочные типы данных - это типы данных, которые описываются в отдельных классах (и отдельных java-файлах). Самым часто используемым классом практически любого языка являются строки. В Java они представлены классом String .

*Подробнее в лекциях:*
лекция “1.5 Типы данных в Java: объекты” из “Блок 1. Основы Java”
  

Т
=======================
 
### Терминал 

Терминал - специальная программа для запуска и выполнения команд операционной системы или других программ. Часто используется как синоним понятия **“консоль”**.

**Пример:** cmd (стандартный терминал в windows), terminal (в linux ), iterm (в macos).
 
 
### Тернарный оператор 

Тернарный оператор - это условный **оператор** без тела кода. Он используется, когда нужно присвоить значение переменной или вернуть значение из метода, не создавая избыточный код (альтернатива условному оператору **if**). Синтаксически конструкция состоит из условия `( условие )` и двух выражений. Выражения от условия отделены знаком вопроса `?`. Между выражениями стоит знак двоеточия `:` . Первое выражение сработает, если условие верно, а второе — если ложно. 

**Пример:** 

    int switchOnRefrigiratorEngine = (refrigeratorTemperature >= 0) ? 1 : 0;

[*Подробнее >*](https://javahelp.online/osnovy/ternarnyy-operator-java)

*Подробнее в лекциях:*
лекция 1.3 Условные операторы и циклы из “Блок 1. Основы Java”.
  

Ц
=======================
 
### Цикл

Цикл — это какое-то повторяющееся действие или набор действий, которые выполняются до тех пор пока не выполнится условие прекращения выполнений (т.е. “выхода из цикла”). Набор повторяющихся в цикле действий называется *“телом цикла”*. Одно повторение входящих в цикл действий называется *«итерация»*.

В java циклы бывают нескольких видов: **for**, **foreach**, **while**, **do while**.

[*Подробнее >*](https://ru.wikipedia.org/wiki/%D0%A6%D0%B8%D0%BA%D0%BB_(%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5))

*Подробнее в лекциях:*
1. лекция 4 (Циклы) из “Блок 0. Введение в Java (Basic Java BJAVA)”,
2. лекция 1.3 Условные операторы и циклы из “Блок 1. Основы Java”.
