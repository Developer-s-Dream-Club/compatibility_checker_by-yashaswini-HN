#include<stdio.h>
#include<string.h>
void main()
{
    char n1[20],n2[20];
    char str[4]="love";
    int i,j,cnt;
    printf(" name1 = ");
    scanf("%s",n1);
    printf(" name2 = ");
    scanf("%s",n2);
    strcat(n2,n1);
    for(i=0;i<20;i++)
    {
        for(j=1;j<5;j++)
        {
            if(n2[i]==str[j])
            cnt++;
        }
    }
    if(cnt<1||cnt>9)
    printf("your love score is %d you go together like coke and mentos",cnt);
    else if(cnt>=4&&cnt<=5)
    printf("your score is %d you are alright together",cnt);
    else
    printf("your score is %d",cnt);
}
