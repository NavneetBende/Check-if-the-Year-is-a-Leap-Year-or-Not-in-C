# Check-if-the-Year-is-a-Leap-Year-or-Not-in-C


Check if the Year is a Leap Year or Not in C
Given an integer input for the year, the objective is to check if the given year input is a leap year or not. To do so we check whether the year is divisible by 400 or not, if true then it’s a leap year, it’s not a leap year otherwise. Therefore we write a program to Check if the Year in a Leap Year or Not in C.

Example
Input : 2020
Output : It's a Leap Year
Check if a Year is a Leap Year or Not in C
Given an integer input for an year, the objective is to check whether the given integer input represents a Leap year or not. In order to do so we’ll check for two conditions, any year to be a leap year must satisfy either of them.

Conditions for a Leap Year
For any year to be a leap year it must satisfy either of these conditions
1. Year must be divisible by 400.
2. Year must be divisible by 4 and not by 100 at the same time.
Why not just check divisibility by 4
Gregorian Calendar
In the Gregorian calendar, a normal year consists of 365 days and a leap year has 366 days. 
Adding 1 extra day every 4 years would mean having on average 365.25 days.
Reason
However, the time required for the Earth to revolve once about the Sun) is actually 365.2425 days
Since, this number is lesser than 365.25. There have to be some years that may be divisible by 4 but won't be treated leap year

Thus scientists set following conditions for a year to be leap year -
1. If a year is divisible by 400
2. If a year is divisible by 4 but not divisible by 100
Based on the above mentioned conditions, we have few methods to Check if a Year is a Leap Year or Not

Method 1: Using if-else Statements 1
Method 2: Using if-else Statements 2
We’ll discuss the above mentioned methods in detail in the sections below.

While loop in C
Related Pages
Sum of numbers in a given range

Greatest of two numbers

Greatest of the Three numbers

Prime number

Prime number within a given range

Method 1: Using if-else Statements 1
In this method we’ll use if-else statements to check for the required conditions for an Year to be a Leap Year.

Working
For a given integer input as year, we do the following

Check if the year variable is divisible by 400. if true it’s a Leap Year, it’s not a Leap Year otherwise.
Check if the year variable is divisible by 4 and not by 100. If true, print it’s a Leap year, It’s not a Leap Year otherwise.
Let’s implement the above mentioned logic in C Language.

C Code
Run
#include <stdio.h>
int main ()
{
    int year;
    year=2000;
    
    if(year % 400 == 0)
        printf("%d is a Leap Year",year);
        
    else if(year % 4 == 0  && year % 100 != 0)
        printf("%d is a Leap Year",year);
        
    else
        printf("%d is not a Leap Year",year);
    
    return 0;
}
Output
2000 is a Leap Year
Method 2: Using if-else Statements 2
In this method we’ll use if-else statements to check for the required conditions for an Year to be a Leap Year. This method is the simplified version of previous method.

Working
For a Given integer input for an year, we check

If the year is divisible by 400. If true it’s a Leap Year, it’s not otherwise.
If the year is divisible by 4 and not by 100. It’s a leap year if true, it’s not otherwise.
Let’s implement the above logic in C Language.

C Code
Run
#include <stdio.h>
int main ()
{
    int year;
    year=2000;
    
    if(year % 400 == 0 || (year % 4 == 0  && year % 100 != 0))
        printf("%d is a Leap Year",year);
        
    else
        printf("%d is not a Leap Year",year);
    
    return 0;
}
Output
2000 is a Leap Year
