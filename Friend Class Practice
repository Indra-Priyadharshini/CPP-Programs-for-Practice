/*Create a person called SalesPerson.
Private Data Members: Eno, Name, Designation, Salescount, Bonus
Public Member Function: readData() - to read data from the user, printData() -To print the details of SalesPerson.
calcBonus()-to calculate bonus based on the following conditions, 
If SalesCount<100, Bonus=1000, if SalesCount is in the range of 100 to 500, Bonus=5000, if SalesCount>500, Bonus=10000.
Friend Class:
Declare a class Salary as a friend to SalesPerson.
Define the class Salary with following members.
Private Data Member: Basic, HRA, DA, PF and Gross
Public Member Functions: readSalary(), printSalary(), calcSalary() - A function that takes SalesPerson class object as argument. 
Calculate HRA=15% of Basic, DA=25% of Basic PF=5% of Basic, Gross=Basic+HRA+DA+Bonus-PF. (Note that Bonus is accessed from SalesPerson Class).
Call the respective functions using necessary objects to print the output to pass testcases.*/

#include <iostream>
using namespace std;
class SP
{
    private:
        int Eno, Salescount, Bonus;
        string Name, Designation;
    public:
        void readData()
        {
            cin>>Eno>>Name>>Designation>>Salescount;
        }
        void calcBonus()
        {
            if (Salescount<100) Bonus = 1000;
            else if (Salescount>500) Bonus = 10000;
            else Bonus = 5000;
        }
        friend void printData(SP sp);
        friend class Salary;
};

class Salary
{
    private:
        int Basic, HRA, DA, PF, Gross;
    public:
        void readSalary()
        {
            cin>>Basic;
        }
        void calcSalary(SP sp)
        {
            HRA = 0.15 * Basic;
            DA = 0.25 * Basic;
            PF = 0.05 * Basic;
            Gross = 1.35 * Basic + sp.Bonus;
        }
        void printSalary()
        {
            cout<<"Basic Salary: "<<Basic<<endl;
            cout<<"HRA: "<<HRA<<endl;
            cout<<"DA: "<<DA<<endl;
            cout<<"PF: "<<PF<<endl;
            cout<<"Gross Salary: "<<Gross<<endl;
        }
};

void printData(SP sp)
{
    cout<<"ID: "<<sp.Eno<<endl;
    cout<<"Name: "<<sp.Name<<endl;
    cout<<"Designation: "<<sp.Designation<<endl;
    cout<<"SalesCount: "<<sp.Salescount<<endl;
    cout<<"Bonus: "<<sp.Bonus<<endl;
}

int main()
{
    SP sp1;
    sp1.readData();
    sp1.calcBonus();
    printData(sp1);
    Salary s1;
    s1.readSalary();
    s1.calcSalary(sp1);
    s1.printSalary();
    return 0;
}
