```c
#include <stdio.h>
#include <locale.h>

int main()
{
    setlocale(LC_ALL, "Ukr");
    float t1, t2, t3, t;
    printf ("Введiть три значення: ");
    scanf ("%f %f %f", &t1, &t2, &t3);
    if (t1 >= 10000 || t2 >= 10000 || t3 >= 10000){
        printf ("Error\n");
        return 0;
    }
    double zag = ((t1 + t2 + t3) / 3) / 3;
    printf ("Час необхідний для з'їдання пирога: %.2f\n", zag );
    return 0;
}
