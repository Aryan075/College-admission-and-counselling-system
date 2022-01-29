# College-admission-and-counselling-system
 
#include <stdio.h>
void intro()
{ 
 printf("\n\t\t\tCOLLEGE ADMISSION COUNSELING\n \t\t\t\tENTER BIO DATA\n\n");
}
void ent()
{ 
 char stream[20];
printf("\n\nENTER THE STREAM YOU WANT TO STUDY\t\t");
scanf("%s",stream);
printf("\n\n \tCONGRATULATIONS!!! YOU HAVE BEEN SELECTED IN %s STREAM",stream);
}
int main () 
 {
 char yourname[20],fname[20],mname[20],state[20],school[30];
 int age,phy,chem,math,t;
 intro();
 printf(" NAME \t\t\t");
 scanf("%s", yourname);
 yourname[19] = '\0';
 fflush(stdin);
 printf(" FATHER'S NAME \t\t");
 scanf("%s", fname);
 fname[19] = '\0';
 fflush(stdin);
 printf("MOTHER'S NAME \t\t");
 scanf("%s", mname);
 mname[19]='\0';
 fflush(stdin);
 printf("STATE OF RESIDENCE \t");
 scanf("%s",state);
 state[19]='\0';
 fflush(stdin); 
 printf(" AGE \t\t\t");
 scanf(" %d",&age);
 printf("SCHOOL NAME\t\t");
 scanf("%s",school);
 school[29]='\0';
 fflush(stdin);
 printf("ENTER PHYSICS MARK \t");
 scanf("%d",&phy);
 printf("ENTER MATH MARK \t");
 scanf("%d",&math);
 printf("ENTER CHEMISTRY MARK \t");
 scanf("%d",&chem);
 t=(phy+math+chem)/3;
 if(t>=50&&t<60)
 {
 printf(" \n\n\t\t %s YOUR GRADE IS E\n\n YOU ARE ELIGIBLE FOR \n\nCIVIL STREAM \nBIOCHEMICAL STREAM \n\nYOU CAN CHOOSE ANY ONE OF THEM \n",yourname);
 ent();
}
else if(t>=60&&t<70)
{
 printf(" \n\n\t\t %s YOUR GRADE IS D\n\n YOU ARE ELIGIBLE FOR \n\nBIOTECHNOLOGY STREAM \nMECHATRONICS STREAM \n\nYOU CAN CHOOSE ANY ONE OF 
THEM\n",yourname);ent() ;
}
 else if(t>=70&&t<80)
 {
 printf(" \n\n\t\t %s YOUR GRADE IS C\n\n YOU ARE ELIGIBLE FOR \n\nBIOTECHNOLOGY STREAM \nMECHANICAL STREAM \n\nYOU CAN CHOOSE ANY ONE OF THEM\n",yourname);
 ent();
}
 else if(t>=80&&t<90)
 {
 printf(" \n\n\t\t %s YOUR GRADE IS B\n\n YOU ARE ELIGIBLE FOR \n\nBIOTECHNOLOGY STREAM\n MECHANICAL STREAM\n ELECTRICAL STREAM \n\nYOU CAN CHOOSE ANY ONE OF THEM 
\n",yourname);
 ent();
}
else if(t>=90&&t<95)
{
 printf(" \n\n\t\t %s YOUR GRADE IS A\n\nYOU ARE ELIGIBLE FOR \n\nBIOTECHNOLOGY STREAM \n MECHANICAL STREAM \nELECTRICAL STREAM \nIT STREAM 
YOU CAN CHOOSE ANY ONE OF THEM ",yourname);ent();}
else if(t>=95&&t<=100)
 {
 printf(" \n\n\t\t %s YOUR GRADE IS A++\n\nYOU ARE ELIGIBLE FOR ALL THE STREAMS OF \n\n BIOTECHNOLOGY STREAM \n MECHANICAL STREAM \nELECTRICAL STREAM \n IT STREAM \n 
ECE STREAM , YOU CAN CHOOSE ANY ONE OF THEM ",yourname);ent();}
 else
 {
 printf(" \n\n\t\t %s YOU GRADES ARE TOO LOW ,\n YOU ARE NOT ELIGIBLE FOR THIS COLLEGE\n\n",yourname);
 }
 return(0);
}
