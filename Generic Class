/*Create a class called Generic with two data members a and b and two generic member functions for reading and printing values.
Sample Output:
a=34 b= 98
a=VIT b=University
a=34.56 98. 09*/
include <iostream>

using namespace std;

template<typename T>
class Generic
{
    private:
        T a, b;
    public:
        void readData()
        {
            cin>>a>>b;
        }
        void printData()
        {
            cout<<"a="<<a<<" b="<<b<<endl;
        }
};

int main()
{
    Generic<int> obj1;
    obj1.readData();
    obj1.printData();
    Generic<string> obj2;
    obj2.readData();
    obj2.printData();
    Generic<float> obj3;
    obj3.readData();
    obj3.printData();
    return 0;
}
