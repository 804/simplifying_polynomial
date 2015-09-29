# 1. Polinomial #
- - - -
Script for submitting expressions containing brackets, one variable, the operations of addition, subtraction, multiplication, and constant degree in expanded form.
- - - -
#### Example: ####

- Input:
(x - 6x^2)(((3 + 6x)(x + 3) - 4x^9000)x - 3)

- Output:
24x^9003 - 4x^9002 - 36x^5 - 120x^4 - 33x^3 + 27x^2 - 3x

```cmd
D:\Data\Python\HHTest2015>python polynom.py

Input expression:
(x - 6x^2)(((3 + 6x)(x + 3) - 4x^9000)x - 3)

Result:
24x^9003 - 4x^9002 - 36x^5 - 120x^4 - 33x^3 + 27x^2 - 3x
```

- - - -
# 2. Infinite sequence #
- - - -
The script for the determination of the first occurrence of input sequences into an infinite sequence formed by gluing consecutive positive integers: S = 123456789101112131415...
- - - -
#### Example: ####

- Input:
002

- Output:
491

```cmd
D:\Data\Python\HHTest2015>python infinite_sequence.py

Input sequence:
002

Result:
491
```
- - - -
- - - -

# 1. Полином #
- - - -
Скрипт для представления выражений, содержащих скобки, одну переменную, операции сложения, вычитания, умножения и возведения в константную степент в развернутом виде.
- - - -
#### Пример: ####

- Ввод:
(x - 6x^2)(((3 + 6x)(x + 3) - 4x^9000)x - 3)

- Вывод:
24x^9003 - 4x^9002 - 36x^5 - 120x^4 - 33x^3 + 27x^2 - 3x

```cmd
D:\Data\Python\HHTest2015>python Polynom.py

Input expression:
(x - 6x^2)(((3 + 6x)(x + 3) - 4x^9000)x - 3)

Result:
24x^9003 - 4x^9002 - 36x^5 - 120x^4 - 33x^3 + 27x^2 - 3x
```

- - - -

# 2. Бесконечная последовательность #
- - - -
Скрипт для определения первого вхождения заданной последовательности в бесконечную цифровую последовательность, образованную склеиванием последовательных положительных чисел: S = 123456789101112131415...
- - - -
#### Пример: ####

- Ввод:
002

- Вывод:
491

```cmd
D:\Data\Python\HHTest2015>python infinite_sequence.py

Input sequence:
002

Result:
491
```
- - - -
- - - -
# Формулировка задач и способы решения #
- - - -
## 1. Полином ##
- - - -
Дано выражение, содержащее скобки, операции сложения, вычитания, умножения, возведения в константную степень и одну переменную, например: (x - 5)(2x^3 + x(x^2 - 9)).

Представьте это выражение в развёрнутом виде, например: 3x^4 - 15x^3 - 9x^2 + 45x
- - - -
### Решение ###
Для решения данной задачи я перевел изначальное выражение в форму обратной польской нотации, а затем провел вычисления, используя для этого приведенные выше операции на многочленах.

- - - -
## 2. Бесконечная последовательность ##
- - - -
Возьмём бесконечную цифровую последовательность, образованную склеиванием последовательных положительных чисел: S = 123456789101112131415...
Определите первое вхождение заданной последовательности A в бесконечной последовательности S (нумерация начинается с 1).

Пример входных данных:
6789
111

Пример выходных данных:
6
12

- - - -
### Решение ###
Для решения данной мне понадобилось ввести такое понятие, как опорный элемент вводимой подпоследовательности. Это число, входящее в склейку при получении бесконечной последовательности, чье начало (хотя бы одна цифра) лежит в вводимой подпоследовательности. Данный элемент оптимально следует искать длиной от 1 цифры до количества цифр, равного длине подпоследовательности. Данный элемент может располагаться от начала подпоследовательности с отступом до его длины (не включая величину самой длины). Если элемент данной длины на данной позиции существует, то после его получения мы вычисляем его позицию в бесконечной последовательности и вычитаем из этой величины отступ. Результатом считается минимальная позиция, вычисленная методом опорных элементов. 
Данное решение оптимальнее, чем обычный проход по последовательности, особенно для большинства подпоследовательностей большой длины, т.к. для этого нам нужно будет проходить не по огромной последовательности, а по той, что мы ввели.
- - - -
- - - -
