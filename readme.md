# Домашнее задание к занятию «Многофайловые проекты и библиотеки»

### Задание 1

[Математические функции](01).

<details>
# Задача 1. Математические функции
В этом задании вы вынесете математические функции в отдельный файл.

Даны следующие математически функции: сложение, вычитание, умножение, деление, возведение в степень.

Вам нужно разместить их в отдельном файле исходного кода и воспользоваться ими из функции `main`.

Попросите пользователя ввести два числа и выбрать операцию. Выведите результат ему на консоль.

### Пример работы программы
#### Консоль
```
Введите первое число: 20
Введите второе число: 2
Выберите операцию (1 - сложение, 2 вычитание, 3 - умножение, 4 - деление, 5 - возведение в степень): 5
20 в степени 2 = 400
```
#### Подсказки

> Не читайте этот раздел сразу. Попытайтесь сначала решить задачу самостоятельно :)

<details>

<summary>Что использовать для решения.</summary>

Для указанных функций создайте два файла — `.cpp` и `.h`.

В заголовочном файле разместите объявления функций.

В файле исходного кода разместите определения функций.

Не забудьте подключить заголовочный файл в соответствующий файл исходного кода и в основной файл.

Не забудьте защиту от двойного подключения в заголовочном файле.

Также для удобства вывода названия фигуры можно создать защищённое поле `name` в классе `Figure` с соответствующим методом `get_name` и заполнением значения в каждом классе. В `Figure` это будет «Фигура» и т. д.

</details>
</details>

### Задание 2

[Класс](02).

<details>
# Задача 2. Класс
В этом задании вы вынесете класс в отдельный файл.

Возьмите класс счётчика из [предыдущего домашнего задания](../../03/02).

Вынесите этот класс в отдельный файл, продемонстрируйте работу программы таким же образом, как в [предыдущем домашнем задании](../../03/02).
 
Вы должны иметь возможность узнать у каждой фигуры длины её сторон и значения её углов, но извне вы не должны быть способны изменить длины сторон и углы.

Не должно быть возможности создать фигуры, не удовлетворяющие перечисленным условиям. Например, нельзя создать квадрат с разными углами. Геометрические соотношения проверять не нужно. Например, сумма углов в треугольнике может быть не равна 180.

Задача: спроектировать и реализовать классы, описывающие предметную область. Продемонстрируйте их работу: создайте по одному экземпляру каждой фигуры и выведите на экран информацию о длинах её сторон и величине её углов. Значения используйте произвольные.

Инициализацию длин сторон и величин углов нужно выполнить с помощью вызова базовых конструкторов.

Для вывода информации о фигуре создайте функцию `print_info`, которая будет принимать в качестве аргумента указатель на базовый класс фигуры.

### Пример работы программы
#### Консоль
```
Вы хотите указать начальное значение счётчика? Введите да или нет: да
Введите начальное значение счётчика: 6
Введите команду ('+', '-', '=' или 'x'): +
Введите команду ('+', '-', '=' или 'x'): +
Введите команду ('+', '-', '=' или 'x'): =
8
Введите команду ('+', '-', '=' или 'x'): -
Введите команду ('+', '-', '=' или 'x'): =
7
Введите команду ('+', '-', '=' или 'x'): x
До свидания!
```
#### Подсказки

> Не читайте этот раздел сразу. Попытайтесь сначала решить задачу самостоятельно :)

<details>

<summary>Что использовать для решения.</summary>

Для указанного класса создайте два файла — `.cpp` и `.h`.

В заголовочном файле разместите определение класса с объявлениями его членов.

В файле исходного кода разместите определения членов класса.

Не забудьте подключить заголовочный файл в соответствующий файл исходного кода и в основной файл.

Не забудьте защиту от двойного подключения в заголовочном файле.

</details>

</details>


### Задание 3

[Иерархия классов](03).

<details>
# Задача 3. Иерархия классов
В этом задании вы вынесете иерархию классов в отдельные файлы.

Возьмите иерархию классов геометрических фигур из [предыдущего домашнего задания](../../05/02).

Разнесите иерархию классов по отдельным файлам, продемонстрируйте работу программы таким же образом, как в [предыдущем домашнем задании](../../05/02).

Обратите внимание на то, что для каждого класса должна быть создана своя пара — заголовочный файл + файл исходного кода.

### Пример работы программы
#### Консоль
```
Фигура:
Правильная
Количество сторон: 0

Треугольник:
Правильная
Количество сторон: 3
Стороны: a=10 b=20 c=30
Углы: A=50 B=60 C=70

Прямоугольный треугольник:
Неправильная
Количество сторон: 3
Стороны: a=10 b=20 c=30
Углы: A=50 B=60 C=90

Прямоугольный треугольник:
Правильная
Количество сторон: 3
Стороны: a=10 b=20 c=30
Углы: A=50 B=40 C=90

Равнобедренный треугольник:
Неправильная
Количество сторон: 3
Стороны: a=10 b=20 c=10
Углы: A=50 B=60 C=50

Равносторонний треугольник:
Правильная
Количество сторон: 3
Стороны: a=30 b=30 c=30
Углы: A=60 B=60 C=60

Четырёхугольник:
Неправильная
Количество сторон: 4
Стороны: a=10 b=20 c=30 d=40
Углы: A=50 B=60 C=70 D=80

Прямоугольник:
Правильная
Количество сторон: 4
Стороны: a=10 b=20 c=10 d=20
Углы: A=90 B=90 C=90 D=90

Квадрат:
Правильная
Количество сторон: 4
Стороны: a=20 b=20 c=20 d=20
Углы: A=90 B=90 C=90 D=90

Параллелограмм:
Неправильная
Количество сторон: 4
Стороны: a=20 b=30 c=20 d=30
Углы: A=30 B=40 C=30 D=40

Ромб:
Неправильная
Количество сторон: 4
Стороны: a=30 b=30 c=30 d=30
Углы: A=30 B=40 C=30 D=40
```
#### Подсказки

> Не читайте этот раздел сразу. Попытайтесь сначала решить задачу самостоятельно :)

<details>

<summary>Что использовать для решения.</summary>

Для каждого класса создайте два файла — `.cpp` и `.h`.

В заголовочном файле разместите определение класса с объявлениями его членов.

В файле исходного кода разместите определения членов класса.

Чтобы унаследовать класс, определённый в другом заголовочном файле, подключите его.

Не забудьте подключить заголовочный файл в соответствующий файл исходного кода и в основной файл.

Не забудьте защиту от двойного подключения в каждом заголовочном файле.

</details>

</details>