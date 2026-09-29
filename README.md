# lab5
```
#define _USE_MATH_DEFINES
#include <math.h>
#include <stdio.h>
#include <locale.h>

int calc()
{
	setlocale(LC_CTYPE, "RUS");

    const double a = 1.0;
    double x, y;
    double num, den, F;

    printf("=============================================================\n");
    printf("Введите значение x: ");
    scanf("%lf", &x);
    printf("Введите значение y: ");
    scanf("%lf", &y);
    printf("=============================================================\n");

    num = 3.0 + exp(y - 1.0);
    den = 1.0 + x * x * fabs(y - tan(a));
    F = num / den;

    printf("Исходные данные:\n");
    printf("a = %.0f (константа)\n", a);
    printf("x = %.6g\n", x);
    printf("y = %.6g\n", y);
    printf("=============================================================\n");
    printf("Результат:\n");
    printf("F(x, y) = %.6f\n", F);
    printf("=============================================================\n");
}

int main()
{
	calc();
	getchar();
	return 0;
}
```
