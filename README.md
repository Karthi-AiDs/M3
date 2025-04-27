# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
    #include <stdio.h>
     #include <math.h>
     
     void calculateEMI(float principal,float annualRate,float tenureYears) {
        
         float tenureMonths = tenureYears * 12;  
         float monthlyRate = (annualRate / (12*100));
         float emi = (principal * monthlyRate * pow(1 + monthlyRate, tenureMonths)) / 
                     (pow(1 + monthlyRate, tenureMonths) - 1);
         
         printf("Monthly EMI is= %.3f", emi);
     }
     
     int main() {
         float principal; 
         float annualRate;   
         float tenureYears;   
         scanf("%f %f %f",&principal,&annualRate,&tenureYears);
         calculateEMI(principal,annualRate,tenureYears);
         return 0;
     }

  

## OUTPUT
![image](https://github.com/user-attachments/assets/1227697d-5aae-4f27-8936-6a1b3555fc04)






## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
    #include<stdio.h>
    void fibonacci(int n)
    {
        int temp=-1,a=1,b=0;
        for (int i=1;i<=n;i++)
        {
            temp=a+b;
            a=b;
            b=temp;
            printf("%d ",a);
           
        }
    }
    int main()
    {
        int num;
        scanf("%d",&num);
        fibonacci(num);
    }
    

## OUTPUT
![image](https://github.com/user-attachments/assets/d65c8db8-36fc-466b-98b7-3d25c10951ac)









## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
    #include<stdio.h>
    int main()
    {
        int n,i;
        scanf("%d",&n);
        int arr[n];
        for (i=0;i<n;i++)
        {
            scanf("%d",&arr[i]);
        }
        if (n>0) printf("%d\n",arr[n-1]);
        else printf(" ");   
    }

## OUTPUT
![image](https://github.com/user-attachments/assets/e68206d7-14e8-4c80-a326-d8c1fb9e86bd)










## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
    #include<stdio.h>
    int main()
    {
        int n,i;
        scanf("%d",&n);
        int arr[n],count_pos=0,count_neg=0;
        for (i=0;i<n;i++)
        {
            scanf("%d",&arr[i]);
            if (arr[i]>0) count_pos++;
            else count_neg++;
        }
        printf("count  of positive numbers  in array: %d\n",count_pos);
        printf("count  of negative numbers  in array: %d",count_neg);
    }



## OUTPUT
![image](https://github.com/user-attachments/assets/07344052-2c31-4cc1-8293-94704f7dfa25)






## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
    #include <stdio.h>
    int main() {
        int arr[100], n, i;
        scanf("%d", &n);
        for(i = 0; i < n; i++) {
            scanf("%d", &arr[i]);
        }
        printf("\nArray after replacing even elements with 'E':\n");
        for(i = 0; i < n; i++) {
            if(arr[i] % 2 == 0) {
                printf("E ");
            } else {
                printf("%d ", arr[i]);
            }
        }
        printf("\n");
        return 0;
    }


## Output:

![Screenshot 2025-04-27 143333](https://github.com/user-attachments/assets/6e6546f0-63c2-4160-8db9-2a8c3e22b6f1)
 
## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.








