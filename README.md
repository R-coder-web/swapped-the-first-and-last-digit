# swapped-the-first-and-last-digit
#include <stdio.h>
#include <math.h>
int main()
{
   int num,digit,first,last,swappedNum;
   printf("enter a number: ");
   scanf("%d",&num);
   last=num%10;
   digit=log10(num);
   first=num/pow(10,digit);
   swappedNum=last*pow(10,digit);
   swappedNum=swappedNum+num% (int)pow(10,digit);
   swappedNum=swappedNum-last;
   swappedNum=swappedNum+first;
   printf("before swapping %d",num);
   printf("after swapping %d",swappedNum);
   
}
