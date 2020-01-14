# 1-Addition
# Simple Calculator Assignment
// Header file for input output functions 
#include <stdio.h> 
#include <stdlib.h> /* atoi */ 
  
  
// Function to compute the sum of two numbers 
int add(int a, int b) 
{ 
    return (a + b) ; 
} 

int diff(int c,int d)
{
	return(c-d);
}

int prod(int a,int b)
{
	return(a*b);
}

int divi(int a,int b)
{
	return(a/b);
}

// Compile this program : g++ addition.cpp -o main 
// When we run a program we can give arguments to that program like:
// ./main 100 200 


int main(int argc, char* argv[]) 
{ 
  
    int num1, num2, num3; 
//argc stands for argument count  
//argv stands for argument values
// These are variables passed to main function when it starts executing
// Check if the length of args array is 1 
    if (argc == 1) 
        printf("No command line arguments found.\n"); 
   else { 
  
// Get the command line argument and 
// Convert it from string type to integer type
// using function "atoi( argument)" 
        num1 = atoi(argv[1]); 
        num2 = atoi(argv[2]); 
  	num3 = atoi(argv[3]);
// Find the average and print it 
        if(num3==1)
	          {
          	printf("%d\n", add(num1, num2)); 
    	      } 
       	else if(num3==2)
	         {
    	      printf("%d\n",diff(num1,num2));
	         }
	      else if(num3==3)
	        {
    	    printf("%d\n",prod(num1,num2));
	        }
	      else if(num3==4)
	       {
    	printf("%d\n",divi(num1,num2));
	       }
	}

	return 0; 
}
 


