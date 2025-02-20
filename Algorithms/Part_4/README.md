# Алгоритмы на графах

- [Цивилизация](./Task%20M.cpp)
- [Свинки-копилки](./Task%20N.cpp)
- [Долой списывание](./Task%20O.cpp)
- [Авиаперелёты](./Task%20P.cpp)

---

## Цивилизация

Карта мира в компьютерной игре «Цивилизация» версии 1 представляет собой прямоугольник, разбитый на квадратики. Каждый квадратик может иметь один из нескольких возможных рельефов, для простоты ограничимся тремя видами рельефов  — поле, лес и вода. Поселенец перемещается по карте, при этом на перемещение в клетку, занятую полем, необходима одна единица времени, на перемещение в лес  — две единицы времени, а перемещаться в клетку с водой нельзя.

У вас есть один поселенец, вы определили место, где нужно построить город, чтобы как можно скорее завладеть всем миром. Найдите маршрут переселенца, приводящий его в место строительства города, требующий минимального времени. На каждом ходе переселенец может перемещаться в клетку, имеющую общую сторону с той клеткой, где он сейчас находится.

### Формат ввода
Во входном файле записаны два натуральных числа N и M, не превосходящих 1000  — размеры карты мира (N  — число строк в карте, M  — число столбцов). Затем заданы координаты начального положения поселенца x и y, где x  — номер строки, y  — номер стролбца на карте (1 ≤ x ≤ N, 1 ≤ y ≤ M), строки нумеруются сверху вниз, столбцы  — слева направо. Затем аналогично задаются координаты клетки, куда необходимо привести поселенца.

Далее идет описание карты мира в виде N строк, каждая из которых содержит M символов. Каждый символ может быть либо «.» (точка), обозначающим поле, либо «W», обозначающим лес, либо «#», обозначающим воду. Гарантируется, что начальная и конечная клетки пути переселенца не являются водой.

### Формат вывода
В первой строке выходного файла выведите количество единиц времени, необходимое для перемещения поселенца (перемещение в клетку с полем занимает 1 единицу времени, перемещение в клетку с лесом  — 2 единицы времени). Во второй строке выходного файла выведите последовательность символов, задающих маршрут переселенца. Каждый символ должен быть одним из четырех следующих: «N» (движение вверх), «E» (движение вправо), «S» (движение вниз), «W» (движение влево). Если таких маршрутов несколько, выведите любой из них.

Если дойти из начальной клетки в конечную невозможно, выведите число -1.

### Пример
| **Ввод** | **Вывод**  |
| :------- | :--------- |
| 4 8 1 1 4 8 | 13 |
| ....WWWW | SSSEENEEEEES |
| .######. |
| .#..W... |
| ...WWWW. |


## Свинки-копилки
У Васи есть n свинок-копилок, свинки занумерованы числами от 1 до n. Каждая копилка может быть открыта единственным соответствующим ей ключом или разбита.

Вася положил ключи в некоторые из копилок (он помнит, какой ключ лежит в какой из копилок). Теперь Вася собрался купить машину, а для этого ему нужно достать деньги из всех копилок. При этом он хочет разбить как можно меньшее количество копилок (ведь ему еще нужно копить деньги на квартиру, дачу, вертолет…). Помогите Васе определить, какое минимальное количество копилок нужно разбить.

### Формат ввода
В первой строке содержится число n — количество свинок-копилок (1 ≤ n ≤ 100). Далее идет n строк с описанием того, где лежит ключ от какой копилки: в i-й из этих строк записан номер копилки, в которой находится ключ от i-й копилки.

### Формат вывода
Выведите единственное число: минимальное количество копилок, которые необходимо разбить.

### Пример
| **Ввод** | **Вывод**  |
| :------- | :--------- |
| 4 | 2 |
| 2 |
| 1 |
| 2 |
| 4 |


## Долой списывание
Во время теста Михаил Дмитриевич заметил, что некоторые лкшата обмениваются записками. Сначала он хотел поставить им всем двойки, но в тот день Михаил Дмитриевич был добрым, а потому решил разделить лкшат на две группы: списывающих и дающих списывать, и поставить двойки только первым.

У Михаила Дмитриевича записаны все пары лкшат, обменявшихся записками. Требуется определить, сможет ли он разделить лкшат на две группы так, чтобы любой обмен записками осуществлялся от лкшонка одной группы лкшонку другой группы.

### Формат ввода
В первой строке находятся два числа N и M — количество лкшат и количество пар лкшат, обменивающихся записками (1 ≤ N ≤ 100, 1 ≤ M ≤ (N * (N - 1)) / 2). Далее в M строках расположены описания пар лкшат: два различных числа, соответствующие номерам лкшат, обменивающихся записками (нумерация лкшат идёт с 1). Каждая пара лкшат перечислена не более одного раза.

### Формат вывода
Необходимо вывести ответ на задачу Павла Олеговича. Если возможно разделить лкшат на две группы, выведите «YES»; иначе выведите «NO».

### Пример
| **Ввод** | **Вывод**  |
| :------- | :--------- |
| 3 2 | YES |
| 1 2 |
| 2 3 |

## Авиаперелёты
Главного конструктора Петю попросили разработать новую модель самолёта для компании «Air Бубундия». Оказалось, что самая сложная часть заключается в подборе оптимального размера топливного бака.

Главный картограф «Air Бубундия» Вася составил подробную карту Бубундии. На этой карте он отметил расход топлива для перелёта между каждой парой городов.

Петя хочет сделать размер бака минимально возможным, для которого самолёт сможет долететь от любого города в любой другой (возможно, с дозаправками в пути).

### Формат ввода
Первая строка входного файла содержит натуральное число n (1 ≤ n ≤ 1000) — число городов в Бубундии. Далее идут n строк по n чисел каждая. j-е число в i-й строке равно расходу топлива при перелёте из i-го города в j-й. Все числа не меньше нуля и меньше 109. Гарантируется, что для любого i в i-й строчке i-е число равно нулю.

### Формат вывода
Первая строка выходного файла должна содержать одно число — оптимальный размер бака.

### Пример
| **Ввод** | **Вывод**  |
| :------- | :--------- |
| 4 | 10 |
| 0 10 12 16 |
| 11 0 8 9 |
| 10 13 0 22 |
| 13 10 17 0 |