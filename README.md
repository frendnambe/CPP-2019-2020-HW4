# CppSource

Repo for fourth homework on 2019/2020 C++ course

# Task 1

Объявить двумерный массив в куче и заполнить его. После заполнения – показать заполненную матрицу на экран и отдельной функцией посчитать сумму элементов отдельно в каждой строке.

Сигнатура функции суммирования:
```cpp
void row_sum(int ** m, unsigned rows, unsigned cols)
{ … }
```

# Task 2

Объявить двумерный массив в куче и заполнить его. После заполнения – показать заполненную матрицу на экран и отдельной функцией посчитать сумму элементов отдельно в каждом столбце. Максимальную сумму вернуть в main().

Сигнатура функции суммирования:
```cpp
int col_sum(int ** m, unsigned rows, unsigned cols)
{ … }
```

# Task 3

Создайте класс Rational с конструктором, принимающим числитель и знаменатель в качестве аргументов. Гарантируется, что знаменатель не равен нулю.

Определите для класса Rational операторы:
 - сложения (`+`), 
 - вычитания (`-`),
 - умножения (`*`),
 - деления (`/`)
 - инкремент (префиксный и постфиксный)
 - декремент (префиксный и постфиксный)
 - сравнения (`>, <, ==, !=, <=, =>`)
 - приведения к `double`

Арифместические операторы должны быть определены так, чтобы экземпляры класса Rational могли использоваться вместе с переменными типа `double` без ограничений.
Операторы сравнения должны быть определены так, чтобы экземпляры класса Rational могли использоваться вместе с переменными типа `int` без ограничений.

Rational в памяти должен храниться в приведенном виде: `10 / 2 => 5 / 1`.

```cpp
class Rational
{
...
private:
	int numerator_;
	int denominator_;
}
```

# Task 3*

Подумайте, что можно сделать, чтобы не переопределять все виды арифметических операторов несколько раз (сначала с двумя Rational, потом с Rational и double, потом с double и Rational).


