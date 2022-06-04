/*Create a class called Sample. Define an integer private data member 'n'. 
Include a default constructor with a cout statement printing "Constructor is Called" and read a value for integer data member.
Include a default destructor with a cout statement printing "Destructor is Called". Create objects in such a way that it displays the following output:

Constructor is Called

Constructor is Called

Constructor is Called

Destructor is Called

Destructor is Called*/

#include <iostream>

using namespace std;

class Sample
{
    private:
        int n;
    public:
        Sample()
        {
            cin>>n;
            cout<<"Constructor is Called"<<endl;
        }
        ~Sample()
        {
            cout<<"Destructor is Called"<<endl;
        }
};

int main()
{
    Sample s1, s5;
    Sample *s = new Sample();
}
