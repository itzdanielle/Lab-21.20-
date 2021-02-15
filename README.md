# Lab-21.20-
//DISPLAY 4.17 Overloading a Function Name
//Illustrates overloading the function name ave.
#include <iostream>
using namespace std;

/*
_Overloading average functions_

Examine the code and verify how the program works. It is similar to Display 4-17 from the book.
Add two more overloaded versions of the avg function. The first new function should return the average of four numbers n1, n2, n3, and n4. The second new function should return the average of five numbers n1, n2, n3, n4, and n5. Call the new functions in the program, similarly to how the current avg functions are demonstrated in main. 
*/

double avg(double n1, double n2);
//Returns the average of the two numbers n1 and n2.

double avg(double n1, double n2, double n3);
//Returns the average of the three numbers n1, n2, and n3.
double avg(double n1, double n2, double n3, double n4);

double avg (double n1, double n2, double n3, double n4, double n5);

int main( )
{
    cout << "The average of 2.0, 2.5, 3.0, 3.5 and 4.0 is "
         << avg(2.0, 2.5, 3.0, 3.5, 4.0) << endl;

    cout << "The average of 2.0, 2.5, 3.0 and 3.5 is "
         << avg(2.0, 2.5, 3.0, 3.5) << endl;

    cout << "The average of 2.0, 2.5, and 3.0 is "
         << avg(2.0, 2.5, 3.0) << endl;

    cout << "The average of 4.5 and 5.5 is "
         << avg(4.5, 5.5) << endl;

}

double avg(double n1, double n2)
{
    return ((n1 + n2)/2.0);
}

double avg(double n1, double n2, double n3)
{
    return ((n1 + n2 + n3)/3.0);
}
double avg (double n1, double n2, double n3, double n4) 
{
   return ((n1 + n2 + n3 + n4)/4.0);
}
double avg (double n1, double n2, double n3, double n4, double n5) 
{
   return ((n1 + n2 + n3 + n4 + n5)/5.0);
}
