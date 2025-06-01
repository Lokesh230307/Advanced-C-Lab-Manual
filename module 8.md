EXP NO:6 C Find a difference between two Numbers Using Pointer in C

Aim:

To write a C program to find the difference between two numbers using pointers.


Algorithm:

1.Start

2.Declare two integer variables and two pointer variables.

3.Accept two integer inputs from the user.

4.Assign the addresses of the variables to the pointer variables.

5.Calculate the difference using pointer dereferencing.

6.Display the result.

7.End

Program:
```
#include<stdio.h>
int main(){
    int a,b,dif;
    int *ptr1,*ptr2;
    scanf("%d %d",&a,&b);
    ptr1=&a;
    ptr2=&b;
    dif=*ptr1-*ptr2;
    printf("%d",dif);
}

```



Output:

![image](https://github.com/user-attachments/assets/9ad954ac-465e-4246-91b1-74acac4e6611)



Result:
Thus, the program is verified successfully
 
EXP NO:7 Given a five digit integer n, print the sum of its digits.

Aim:

To write a C program that takes a five-digit integer as input and prints the sum of its digits.

Algorithm:

Start

Declare an integer variable n and sum = 0.

Read the five-digit integer from the user.

Use a loop to extract each digit (using % and /) and add it to sum.

After the loop, print the sum.

End


 
Program:
```
#include<stdio.h>
int main()
{
    int a,n,sum=0;
    scanf("%d",&a);
    while(a>0){
        n=a%10;
        sum=n+sum;
        a/=10;
    }
    printf("%d",sum);
}
```

Output:


![image](https://github.com/user-attachments/assets/1dca8454-f3b0-4609-b459-602c7054a1f2)







Result:
Thus, the program is verified successfully

EXP NO:8 C PROGRAM TO PRINT ALL OF ITS PERMUTATIONS IN STRICT LEXICOGRAPHICAL ORDER.
Aim:
To write a C program to print all of its permutations in strict lexicographical order.

Algorithm:
1.	Start
2.	Declare variables s (pointer to an array of strings) and n (number of strings)

3.	Memory Allocation
Dynamically allocate memory for s to store an array of strings
4.	Input
Read the number of strings n from the user Dynamically allocate memory for each string in s
5.	Permutation Generation Loop
6.	Memory Deallocation
Free the memory allocated for each string in s Free the memory allocated for s
7.	End
 
Program:

```
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    char arr[50][50];
    for(int i=0;i<n;i++)
    {
        scanf("%s",arr[i]);
    }
    if(n==2)
    {
        printf("%s %s\n",arr[0],arr[1]);
        printf("%s %s",arr[1],arr[0]);
    }
    else
    {
        for(int i=0;i<n;i++)
        {
            for(int j=0;j<n;j++)
            {
                for(int k=0;k<n;k++)
                {
                    if(i!=j && j!=k && k!=i)
                    {
                        printf("%s %s %s\n",arr[i],arr[j],arr[k]);
                    }
                }
            }
        }
    }
}

```
Output:




![image](https://github.com/user-attachments/assets/e2d51c66-afda-4f34-aa0c-af0918879d9a)




Result:
Thus, the program is verified successfully
 
EXP NO:9 C PROGRAM PRINT A PATTERN OF NUMBERS FROM 1 TO N AS
SHOWN BELOW.
Aim:
To write a C program to print a pattern of numbers from 1 to n as shown below.
Algorithm:
1.	Start
2.	Declare integer variables n, i, j, min
3.	Read the value of n from the user
4.	Calculate the length of the side of the square matrix: len = n * 2 - 1
5.	Matrix Generation Loop
6.	Calculate min as the minimum distance to the borders
7.	End
 
Program:

```

#include<stdio.h>
int main()
{
    int n,min;
    scanf("%d",&n);
    for(int i=0;i<2*n-1;i++)
    {
        for(int j=0;j<2*n-1;j++)
        {
            min=i;
            if(j<min)min=j;
            if((2*n-2-i)<min)min=(2*n-2-i);
            if((2*n-2-j)<min)min=(2*n-2-j);
            printf("%d ",n-min);
        }
         printf("\n");
       
    }
}
```
Output:



![WhatsApp Image 2025-04-27 at 15 23 23_3f410c3f](https://github.com/user-attachments/assets/d7bd8d7f-3504-4519-bda7-0cbc944b44c3)





Result:
Thus, the program is verified successfully

EXP NO:10 C PROGRAM TO FIND A SQUARE  OF NUMBER USING FUNCTION WITHOUT ARGUMENTS WITH RETURN TYPE

Aim:

To write a C program that calculates the square of a number using a function that does not take any arguments, but returns the square of the number.

Algorithm:

1.	Start.
2.	Define a function square() with no parameters. This function will return an integer value.
3.	Inside the function:
o	Declare an integer variable to store the number.
o	Ask the user to input a number.
o	Calculate the square of the number (multiply the number by itself).
o	Return the squared value.
4.	In the main function:
o	Call the square() function and display the result.
5.	End.

Program:
```
#include <stdio.h>
int square() 
{
    int num;
    scanf("%d", &num);
    return num * num;
}

int main() 
{
    int result;
    result = square(); 
    printf("The square of the number is: %d\n", result);
    return 0;
}

```



Output:


![WhatsApp Image 2025-04-26 at 11 53 18_1a454ed9](https://github.com/user-attachments/assets/2d213a78-37ce-41bd-9894-2d973f71999a)







Result:
Thus, the program is verified successfully



























