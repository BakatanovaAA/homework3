# Домашнее задание к работе 3
## Условие задачи

Написать и отладить программу вычисления площади и периметра прямоугольника со сторонами A и B, указанными пользователем.

**Вариант 2**

---

## Алгоритм

1. **Начало**
2. Ввести стороны `a` и `b`
3. Вычислить площадь: `area = a * b`
4. Вычислить периметр: `perimeter = 2 * (a + b)`
5. Вывести `area` и `perimeter`
6. **Конец**

## Код

```c
#define _CRT_SECURE_NO_DEPRECATE
#include <locale.h>
#include <stdio.h>
#include <stdlib.h>

double calc_area(double a, double b);
double calc_perimeter(double a, double b);

int main()
{
    double a, b, area, perimeter;

    setlocale(LC_ALL, "RUS");

    puts("Введите сторону A");
    scanf("%lf", &a);
    puts("Введите сторону B");
    scanf("%lf", &b);

    area = calc_area(a, b);
    perimeter = calc_perimeter(a, b);

    printf("Площадь = %.2f\n", area);
    printf("Периметр = %.2f\n", perimeter);

    system("pause");
    return 0;
}

double calc_area(double a, double b)
{
    double area;
    area = a * b;
    return area;
}

double calc_perimeter(double a, double b)
{
    double perimeter;
    perimeter = 2 * (a + b);
    return perimeter;
}
```

## Результат

```
Введите сторону A
578
Введите сторону B
3465
Площадь = 2002770,00
Периметр = 8086,00
```
