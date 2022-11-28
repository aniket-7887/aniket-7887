#include <stdio.h>

int main()
{
    int evenSum=0, oddSum=0;
    void addition(int* , int*);
    addition(&evenSum, &oddSum);
    printf("Addition of first 20 even numbers is %d",evenSum);
    printf("\nAddition of first 20 odd numbers is %d",oddSum);
    return 0;
}
void addition(int* evenSum,int* oddSum)
{
    int i;
    for(i=2;i<=20;i+=2)
    {
        *evenSum+=i;
    }
    for(i=1;i<=20;i+=2)
    {
        *oddSum+=i;
    }
}
