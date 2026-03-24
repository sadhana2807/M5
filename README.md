EX-21-POINTERS
# AIM:
Write a C program to convert a 100.50 into 100 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (100.50).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
~~~
#include<stdio.h>
int main(){
    float n;
    float *p;
    int result;
    scanf("%f",&n);
    p=&n;
    result=(int)(*p);
    printf("the integer equivalent of %.2f =%d",*p, result);
    
}
~~~
<img width="1061" height="598" alt="image" src="https://github.com/user-attachments/assets/fddd0451-07ab-45c1-9de5-35d01b5d2bcb" />


## OUTPUT:
 	
<img width="1118" height="233" alt="image" src="https://github.com/user-attachments/assets/9c7b8747-ec19-4bbc-9759-b3367a7d2cf5" />





## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
~~~
#include <stdio.h>
long long int product(int n){
    if(n==1){
        return 1;
    }else{
        return n*product(n-1);
    }
}
int main(){
    long long int result;
    result=product(12);
    printf("Product is = %lld",result);
    return 0;
}
~~~
<img width="1020" height="655" alt="image" src="https://github.com/user-attachments/assets/fcdcc845-85f9-45ed-801f-0e31ba4355c4" />

## OUTPUT:
<img width="873" height="181" alt="image" src="https://github.com/user-attachments/assets/ceee5066-8a14-402d-ab90-c781d676e363" />

         		
## RESULT:

Thus the program has been executed successfully.
 
 


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each column of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each column of the matrix.
3.	Inside the loop, calculate the sum of the elements in each column.
4.	Print the sum for each column.

## PROGRAM:
~~~
#include <stdio.h>

int main()
{
    int r,c;
    scanf("%d %d",&r,&c);
    int a[r][c];
    for(int i=0;i<r;i++){
        for(int j=0;j<c;j++){
            scanf("%d",&a[i][j]);
        }
    }
    for(int j=0;j<c;j++){
        int sum=0;
        for(int i=0;i<r;i++){
            sum=sum+a[i][j];
        }
        printf("The Sum of Elements of a Column in a Matrix:  %d\n",sum);
    }
    

    return 0;
}
~~~
<img width="757" height="862" alt="image" src="https://github.com/user-attachments/assets/f1bbe250-eb57-4ae0-bef7-b1131c73e5b2" />




## OUTPUT

<img width="962" height="274" alt="image" src="https://github.com/user-attachments/assets/80219ca0-87ca-4f19-b558-63e649e1bae8" />

 
 

 ## RESULT
 Thus the program has been executed successfully.


# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:
~~~


 ## OUTPUT

 

## RESULT

Thus the C program to String process executed successfully
 

 
.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM

## OUTPUT

 

## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


