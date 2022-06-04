/*Ken sports academy conducts summer coaching classes every year on sports like cricket, badminton, swimming, skating,…. 
They plan to collect details of the candidates joining their summer camp with the fields such as name of the candidate, age, game1, hours1, game2, hours2, game3, hours3,
Later they realized that the number of fields are more with no data. Hence they classified it into two classes with the following field set. 
Write a program in C++ to help the organization to maintain the database with relevant base and derived classes.

General - candidateid, name, age, packageamouunt
Customized - candidateid, name, age, no.ofgames, no.ofhours, totalamount */
#include <iostream>

using namespace std;

class Base
{
    private:
        int age, pam;
        string name;
    public:
        static int id;
        virtual void getData()
        {
            cin>>age>>pam>>name;
        }
        virtual void putData()
        {
            cout<<"Age="<<age<<endl;
            cout<<"Package Amount="<<pam<<endl;
            cout<<"name="<<name<<endl;
            cout<<"id="<<id<<endl;
        }
};

class Derived: public Base
{
    private:
        int ta, g, h;
    public:
        Derived()
        {
            id++;
        }
        void getData()
        {
            cin>>g>>ta>>h;
        }
        void putData()
        {
            cout<<"No.of Games="<<g<<endl;
            cout<<"Total amount="<<ta<<endl;
            cout<<"No.of hours="<<h<<endl;
        }
        
};

int Base::id = 0;

int main()
{
    Base *bptr;
    
    Base b1;
    bptr = &b1;
    bptr->getData();
    Derived d1;
    bptr = &d1;
    bptr->getData();
    
    bptr = &b1;
    bptr->putData();
    bptr = &d1;
    bptr->putData();
    
    return 0;
}
