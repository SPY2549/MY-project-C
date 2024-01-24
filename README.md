#include <stdio.h>
#include <stdlib.h>
void swap (int*a,int*b) {
   int temp=*a;
    *a=*b;
    *b = temp;

}
int main()
{
    int num1,num2,num3;
    printf("กรุณากรอกข้อมูลตัวเลข3จำนวน");
    scanf("%d %d %d",&num1,&num2,&num3);

    if (num1>num2) {
        swap(&num1,&num2);
    }
    if (num2>num3) {
        swap(&num2,&num3);
    }
    if (num1>num2){
        swap(&num1,&num2);
    }
    printf("output=%d %d %d \n" ,num1,num2,num3);
}
