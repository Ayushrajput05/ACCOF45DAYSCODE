# ACCOF45DAYSCODE#include <stdio.h>
struct student
{
char name[60];
int roll,age;
float fees,gpa;
};
void main()
{
int i;
struct student s={"Anil Sharma",1,19,7.9,98000};
struct student stud[10];
printf("\n *******DETAILS OF STUDENTS**********");
    printf("\nRollno=%d",s.roll);
    printf("\nName=%s",s.name);
    printf("\nFee=%.1f",s.gpa);
    printf("\nAge=%d",s.age);
    printf("\nFees=%.2f",s.fees);
for(i=0;i<3;i++)
{
    printf("\n Enter roll number:");
    scanf("%d",&stud[i].roll);
    printf("\n Enter name:");
    scanf("%s",stud[i].name);
    printf("\n Enter fees:");
    scanf("%f",&stud[i].fees);
    printf("\n Enter Age:");
    scanf("%d",&stud[i].age);
    printf("\n Enter GPA:");
    scanf("%f",&stud[i].gpa);
}
printf("\n *******DETAILS OF STUDENTS**********");
for(i=1;i<3;i++)
{
    printf("\n Rollno=%d",stud[i].roll);
    printf("\n Name=%s",stud[i].name);
    printf("\n Fee=%.1f",stud[i].gpa);
    printf("\n Age=%d",stud[i].age);
    printf("\n Fee=%.2f",stud[i].fees);
}
    return 0;
}
