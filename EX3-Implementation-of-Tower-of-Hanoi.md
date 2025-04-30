# EX3 Implementation of Tower of Hanoi
## DATE:
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1.Start the program.
2.Define the function TOH(n, source, auxiliary, destination).
3.Inside the function, check if n > 0: a. Recursively call TOH(n-1, source, destination, auxiliary) to
move n-1 disks from the source rod to the auxiliary rod. b. Print the move of the nth disk from the
source rod to the destination rod. c. Recursively call TOH(n-1, auxiliary, source, destination) to move
n-1 disks from the auxiliary rod to the destination rod.
4.Initially call the function with TOH(n, 'A', 'B', 'C'), where 'A', 'B', and 'C' represent the rods.
5.End the program.

## Program:
/*
Program to implement Tower of Hanoi
Developed by: ARULARASI 
RegisterNumber:212223100002  
*/
```
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
if(n>0)
{
TOH(n-1,x,z,y);
printf("%c to %c",x,y);
printf("\n");
TOH(n-1,z,y,x);
}
}
int main()
{
int n=2;
TOH(n,'A','B','C');
}

```

## Output:

![image](https://github.com/user-attachments/assets/b0e0e418-b341-4e04-9207-12ab7e7f7845)


## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
