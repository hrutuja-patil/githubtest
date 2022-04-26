#include<stdio.h>
int main() {
int num,rem,reverse_num,temp,start,stop;
printf ("enter the lower limit:");
scanf("%d",&start);
printf("enter the upper limit");
scanf("%d",&stop);

printf("Palindrome numbers between %d and %d are:",start,stop);

for(num=start;num<=stop;num++){
    temp=num;
    reverse_num=0;
    while(temp){
       rem=temp%10;
       temp=temp/10;
       reverse_num=reverse_num*10+rem;
       }
       if (num==reverse_num)
         printf("%d",num);
   }
  return 0;  
}











