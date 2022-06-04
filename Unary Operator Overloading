/*Class: Sample
Private Data Memers: x, y
Public Member Functions:
readData(), printData(), Sample()
Overlaod -- operator (Pre Decrement), and Unary Minus (-) operator.
Write main functions to create two objects S1 and S2. Call relevant member functions to read and print the output.
Sample Input
5 8
4 6
Sample Output:
4 7
-4 -6*/

#include <iostream>

using namespace std;

class Sample
{
    private:
        int x, y;
    public:
        Sample();
        void readData();
        void printData();
        Sample operator --();
        Sample operator -();
};

Sample::Sample()
{
    x = 0;
    y = 0;
}
void Sample::readData()
{
    cin>>x>>y;
}
void Sample::printData()
{
    cout<<x<<" "<<y<<endl;
}
Sample Sample::operator --()
{
    x -= 1;
    y -= 1;
}
Sample Sample::operator -()
{
    x *= -1;
    y *= -1;
}

int main()
{
    Sample s1, s2;
    s1.readData();
    --s1;
    s1.printData();
    s2.readData();
    -s2;
    s2.printData();
    return 0;
}
