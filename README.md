# Class-project-1
Write a program that inputs one five-digit number, separates the number into its individual digits
and prints the digits separated from one another by three spaces each. 
[Hint: Use combinations of integer division and the remainder operation.] 
For example, if the user types in 45139, the program should print: 4 5 1 3 9


//Momin Hussain
//UCF COP3223c-Spring2018
//HW1 Question7

#include "stdio.h"

int main(void) 
{
  int number, a, b, c, d, e; //We will use 5 letters to represent each digit
  
  printf( "Type a 5 digit number: \n" ); //Tell user to type a 5 digit number
  scanf( "%d", &number );
  
  a = number / 10000;
  b = number / 1000 % 10;
  c = number / 100 % 10;
  d = number / 10 % 10;
  e = number % 10;
  // Each letter will represent a different decimal place
  // For example, a is the ten thousandths place and c is the hundredths place.
  
  printf("%d %d %d %d %d\n ", a, b, c, d, e);
  return 0;
}

// End of Question 7

