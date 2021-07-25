#include <iostream> 
using namespace std; 

char if_grade(int Num) 
{ 
char Grade; 
if ((Num < 0) || (Num > 10))
Grade = 'N';
else if (Num >= 9)
Grade = 'A';
else if (Num >= 8)
Grade = 'B';
else if (Num >= 7)
Grade = 'B';
else if (Num >= 6)
Grade = 'C';
else if (Num >= 5)
Grade = 'C'; 
else if (Num >= 4)
Grade = 'D';
else
Grade = 'F';
return(Grade);
}

char switch_grade(int Num) 
{ 
char grade;
switch(Num)
{
case 0: 
case 1: 
case 2: 
case 3: 
case 4: 
case 5: 
grade = 'F'; 
break; 
case 6: 
grade = 'D'; 
break; 
case 7: 
grade = 'C'; 
break; 
case 8: 
grade = 'B'; 
break; 
case 9: 
case 10: 
grade = 'A';
break; 
}
return(grade);
}

int main() 
{ 
int number; 
cout << " Please enter an integer from 0-10" << endl; 
cin >> number; 
char grades = if_grade(number); 
char switch_grades= switch_grade(number); 
cout << " The grade is: " << grades << endl; 
system("pause");
return 0;
}
