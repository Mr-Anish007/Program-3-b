# Program-3-b
## C-Module 3
## EX_NO-03)b)-Looping
### Date: 19-10-2025
### Name: Anish D
### Register Number:25010086
## AIM:
Create a C program  to check whether the given number is Armstrong number or not.
## ALGORITHM:
1. Start the program.
2. Declare integer variables: num, var, var1, and sum. Initialize sum to 0.
3. Read an integer value num from the user using scanf.
4. Assign the value of num to var.
5. Use a while loop that runs as long as var is not equal to 0:

    a. Extract the last digit of var using var % 10 and store it in var1.

    b. Add the cube of var1 to sum using pow(var1, 3).

    c. Remove the last digit from var by dividing it by 10.

6. After the loop, check if sum is equal to num:

   a. If true, print that num is an Armstrong number.

    b. If false, print that num is not an Armstrong number.

7. End the program.

## PROGRAM:
```
#include<stdio.h>
#include<math.h>
int main()
{
    int num,var,var1,sum=0;
    scanf("%d",&num);
    var=num;
    while(var !=0)
    {
      var1=var%10;
      sum+=pow(var1,3);
      var/=10;
    }
    if(num==sum)
    printf("%d is armstrong number",num);
    else
    printf("%d is not a armstrong number",num);
}
```
## OUTPUT:
<img width="854" height="305" alt="Screenshot 2025-10-19 221532" src="https://github.com/user-attachments/assets/b8561f63-0069-4eb8-b33b-79cd625732c0" />

## RESULT:
Thus the program to check whether the given number is Armstrong number or not has been executed successfully
