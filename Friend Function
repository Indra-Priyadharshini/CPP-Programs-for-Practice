/*
#include <iostream>
Create a person called SalesPerson.
Private Data Members: Eno, Name, Designation, Salescount, Bonus
Public Member Function: readData() - to read data from the user, calcBonus()-to calculate bonus based on the following conditions,
If SalesCount<100, Bonus=1000, if SalesCount is in the range of 100 to 500, Bonus=5000, if SalesCount>500, Bonus=10000.
Friend Function: printData() -To print the details of SalesPerson.*/

#include <iostream>
using namespace std;
class SP
{
    private:
        long Eno, Salescount, Bonus;
        string Name, Designation;
    public:
        void readData()
        {
            cin>>Eno>>Name>>Designation>>Salescount;
        }
        void calcBonus()
        {
            if (Salescount<100) Bonus = 1000;
            else if (Salescount>500) Bonus = 15000;
            else Bonus = 10000;
        }
        friend void printData(SP sp);
};

void printData(SP sp)
{
    cout<<"ID: "<<sp.Eno<<endl;
    cout<<"Name: "<<sp.Name<<endl;
    cout<<"Designation: "<<sp.Designation<<endl;
    cout<<"SalesCount: "<<sp.Salescount<<endl;
    cout<<"Bonus: "<<sp.Bonus;//<<endl;
}

int main()
{
    SP sp1;
    sp1.readData();
    sp1.calcBonus();
    printData(sp1);
    return 0;
}
