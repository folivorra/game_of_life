# The Game Of Life (school21)

## Introduction

На языке программирования Си была разработана программа, представляющая собой визуализацию «The Game of Life». Для отображения графики были использованы только символьная (ASCII) графику (с выводом в терминал). Игра была реализована  в интерактивном режиме, c настройкой скорости игры.

***Графика:***
- Поле — прямоугольник 80 на 25 клеток.
>Подразумевается, что поле «замкнуто само на себя», к примеру у нижнего правого квадратика соседом справа является нижний левый квадратик, а соседом снизу - верхний правый.
- Живая клетка - '0', мертва клетка - '-'.

***Управление:***
- Ускорить время - 'x', замедлить время - 'z'.
- Выход - 'q'.

***Концовки игры:***
- Пользователь сам решил выйти с помощью соответствующей клавиши.
- Популяция больше не будет развиваться, т.е. образовались статичные вечные фигуры.
- Популяция вымерла.

Было подготовлено 5 файлов с начальными состояниями для перенаправления потока в stdin (находятся в папке assets). 

## Build and run

```bash
$ gcc -Wall -Werror -Wextra -lncurses game_of_life.c -o gol.out
$ ./gol.out < assets/[name_of_asset_file]
```