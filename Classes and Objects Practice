/*Create a class called Point with following specifications:

Private Integer Data members: X and Y

Constructors: Default constructor and Parameterized constructor with two arguments

Public member functions: 1) readData() - to read values for X and Y from user 
2) printData() - to print X and Y values 3) addData() - to sum up X and Y and display the sum

Objects: 1) Create Obj1 with no arguments, read values from user, print values and sum. 2) Create obj2 with arguments 35 and 70, print values and sum*/

#include <iostream>

using namespace std;

class Point
{
    private:
        int x, y;
    public:
        Point()
        {
            
        }
        Point(int a, int b)
        {
            x = a; y = b;
        }
        void readData()
        {
            cin>>x>>y;
        }
        void printData()
        {
            cout<<"X="<<x<<endl<<"Y="<<y<<endl;
        }
        void addData()
        {
            cout<<"Sum="<<x+y<<endl;
        }
};

int main()
{
    Point p1;
    p1.readData();
    p1.printData();
    p1.addData();
    Point p2(35, 70);
    p2.printData();
    p2.addData();
    return 0;
}
