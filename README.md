# pattern-print.c
// c program to print pattern with spaces      E    DE D   CDE  DC  BCDE   DCB ABCDE    DCBA  
// c program to print pattern with spaces

     E
   DE D
  CDE DC
 BCDE DCB
ABCDE DCBA

#include <stdio.h>
int main() { 
    int i,j;
    for(i=0;i<5;i++)
    {
        for(j=0;j<=3-i;j++)
         printf(" ");
        for(j=4-i;j<=4;j++)
         printf("%c",65+j);
        for(j=0;j<=i-1;j++)
         printf(" ");
        for(j=3;j>=4-i;j--)
         printf("%c",65+j);
        printf("\n");
    }
    return 0;
}
