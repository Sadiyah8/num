#include<stdio.h>
int main()
{
int present_capacity,rated_capacity,ch=0,ce=0,cf=0;
int SoH;
scanf("%d%d",&present_capacity,&rated_capacity);
  if(rated_capacity==0)
  {
    printf("Error");
    return 1;
  }
  
SoH=(100*present_capacity)/rated_capacity;
if(SoH>80 && SoH<=100)
ch++;
else if(SoH>=63 && SoH<=80)
  ce++;
else
  cf++;
printf("%d %d %d",ch,ce,cf);
  return 0;
}
