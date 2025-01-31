// write a prgm to calculate the sum of two complex numbers
// x = 1+2i, y = 2+3i
#include <stdio.h>
typedef struct complexnumber{
    int real;
    int img;
}complex;
complex add(complex x, complex y)
{
    complex add;
    add.real = x.real+y.real;
    add.img = x.img+y.img;
    return (add);
}
int main(){
    complex x,y,sum;
    x.real = 1;
    x.img = 2;
    y.real = 2;
    y.img = 3;
    printf("x=%d +%di\n", x.real, x.img);
    printf("y=%d +%di\n", y.real, y.img);
    sum = add(x,y);
    printf("\n sum = %d + %di", sum.real, sum.img);
    return 0;
}
