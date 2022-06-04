/*Class name: Employee
Private Memers: Eno,Ename,Age,BasicSalary, checkAge() - To check whether the age is in the range 22 to 58, if it is beyond 58, make it 58.
If it is less than 22, make it 22.
Public Members: default constructor-initialize with default values, readData() - read user data,
printData()-display the basic employee details also check the age limit, 
calcPayroll() - Function to calculate and display HRA, DA, PF,Gross,Netsal (HRA-10% of basic, DA-30% of basic, 
PF-5% of basic, Gross is sum of basic,HRA,and DA, Netsal is subtracting PF from Gross.) 
Create an object in main function and call the member functions.*/

#include <iostream>
#include <string>

using namespace std;

class Employee
{
    private:
        int Eno, Age, BasicSalary;
        string Ename;
        
        void checkAge()
        {
            if (Age>58) Age = 58;
            else if (Age<22) Age = 22;
        }
    public:
        Employee(int num = 1, int age = 22, int bs = 1000, string name = "Ashok")
        {
            Ename = name;
            Eno = num;
            Age = age;
            BasicSalary = bs;
        }
        void readData()
        {
            cin>>Eno>>Ename>>Age>>BasicSalary;
            checkAge();
        }
        void printData()
        {
            cout<<"Emp No: "<<Eno<<endl;
            cout<<"Emp Name: "<<Ename<<endl;
            cout<<"Emp Age: "<<Age<<endl;
            cout<<"Basic Salary: "<<BasicSalary<<endl;
        }
        void calcPayroll()
        {
            float hra = 0.1 * BasicSalary, da = 0.3 * BasicSalary, pf = 0.05 * BasicSalary, gross = 1.4 * BasicSalary, netsal = 1.35 * BasicSalary;
            cout<<"HRA: "<<hra<<endl;
            cout<<"DA: "<<da<<endl;
            cout<<"PF: "<<pf<<endl;
            cout<<"Gross Salary: "<<gross<<endl;
            cout<<"Net Salary: "<<netsal<<endl;
        }
};

int main()
{
    Employee e1;
    e1.readData();
    e1.printData();
    e1.calcPayroll();
    return 0;
}
