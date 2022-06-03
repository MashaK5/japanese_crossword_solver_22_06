# Решатель японских кроссвордов


### Запуск программы:

```Console
cabal new-run hw-mathlog2202
```

### Формат ввода:

Обратите внимание, что вывод работает корректно только для таблице со сторонами меньше 10.

Программа выведет сообщение **Enter the number of rows:**, после чего надо ввести количество строк кроссворда - натуральное число. 

При некорректном количестве строк программа выведет сообщение **Invalid rows input! All elements must be natural numbers separated by spaces.** и остановит выполнение программы.

Далее программа выведет сообщение **Enter the specified number of lines:**, после чего надо ввести указанное ранее количество строк, где каждая строка - последовательность натуральных чисел, разделенных пробелами.

При некорректном вводе программа выведет сообщение **Invalid rows input! All elements must be natural numbers separated by spaces.** и остановит выполнение программы.

Каждое число в строке означает обособленную группу закрашенных в этой строке. Размер группы может быть 0, только если эта группа в строке единственная. Именно нулем следует обозначать строку, в которой нет закрашенных клеток.
В случае неправильного применения числа 0 будет выведено следующее сообщение **Invalid rows input! There is a string of several numbers with zero element.**. В случае ввода пустой строки будет выведено сообщение **Invalid rows input! There is an empty line of rules.**


Далее следует аналогичный ввод столбцов.

В конце ввода программа проверяет, что введенные условия коректны и не противоречат друг другу. При некорректных условиях программа выведет **Invalid rows input! Some line is too long.** или **Invalid colums input! Some line is too long.**


### Формат вывода:

Выводится классический вид японского кроссворда с решением, если оно есть.
И `Unsatisfiable` если решение не существует.


### Пример:

```Console
Enter the number of rows:
5
Enter the specified number of lines:
2
1 1
1
3
1 1
Enter the number of columns:
4
Enter the specified number of lines:
1
4
1 1
2 1

  ║ ║ ║1║2║
  ║1║4║1║1║
══╬═╬═╬═╬═╣
 2║ ║ ║+║+║
══╬═╬═╬═╬═╣
11║ ║+║ ║+║
══╬═╬═╬═╬═╣
 1║ ║+║ ║ ║
══╬═╬═╬═╬═╣
 3║+║+║+║ ║
══╬═╬═╬═╬═╣
11║ ║+║ ║+║
══╩═╩═╩═╩═╝
```




