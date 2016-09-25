# Interpretador-em-C
#include<stdio.h>
#include<string.h>

int main(int argc, char *argv[])
{
    int num1, num2;
    int error=0;
    printf("Interpretador em C:\n");

    if(strcmp(argv[1],"ADD")==0)
    {
        num1 = atoi(argv[2]);
        num2 = atoi(argv[3]);
        printf("[%d]\n", num1+num2);
        error++;
    }
    if(strcmp(argv[1],"SUB")==0)
    {
        num1 = atoi(argv[2]);
        num2 = atoi(argv[3]);
        printf("[%d]\n", num1-num2);
        error++;
    }
    if(strcmp(argv[1],"MULT")==0)
    {
        num1 = atoi(argv[2]);
        num2 = atoi(argv[3]);
        printf("[%d]\n", num1*num2);
        error++;
    }
    if(strcmp(argv[1],"DIV")==0)
    {
        num1 = atoi(argv[2]);
        num2 = atoi(argv[3]);
        printf("[%d]\n", num1/num2);
        error++;
    }
    if(strcmp(argv[1],"AND")==0)
    {
        num1 = atoi(argv[2]);
        num2 = atoi(argv[3]);
        printf("[%d]\n", num1&num2);
        error++;
    }
    if(strcmp(argv[1],"OR")==0)
    {
        num1 = atoi(argv[2]);
        num2 = atoi(argv[3]);
        printf("[%d]\n", num1|num2);
        error++;
    }
    if(error==0)
    {
        printf("ERROR: INVALID OPERATION\n");
    }



}
