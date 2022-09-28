#include <stdio.h>
#include <math.h>
#include <time.h>
#include <stdlib.h>

float a[5];
float num;
int b;
float c;
int d;

void main()
{
    scanf("%f", &num);
    srand(time(NULL)+rand());
    for(b = 1; b <= 5; ++b)
    {
        a[b] = num;
        c = 0;
        if (rand() % 2 != 0) c = (a[b]-(rand() % 10)) / 1000;
        else  c = (a[b]+(rand() % 10)) / 1000;
        printf("%f ", c);
    }
}
