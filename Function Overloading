/*Create a class called Employee. Define the class data members for storing necessary attributes. Define necessary member functions to read and print the attributes. 
Define a member function calculateGross() and oveload it in the following manner.
1) If only basic salary is provided as argument, calculate the gross salary as basic+5000.
2) If basic and HRA are provided as arguments, calculate the gross salary as basic+5000+HRA 
3) If basic, HRA and DA are provided as arguments, calculate the gross salary as basic+5000+DA+HRA 
4) If basic, HRA, DA and TA are provided as arguments, calculate the gross salary as basic+5000+DA+HRA+TA.*/

#include <iostream>

using namespace std;

class Employee
{
    private:
        int no;
        string name;
    public:
        Employee()
        {
            cin>>no>>name;
        }
        void printData()
        {
            cout<<"Employee Numer: "<<no<<endl;
            cout<<"Employee Name: "<<name<<endl;
        }
        void calculateGross(int basic)
        {
            cout<<"Basic: "<<basic<<endl<<"Gross Salary: "<<basic + 5000<<endl<<"***"<<endl;
        }
        void calculateGross(int basic, int hra)
        {
            cout<<"Basic: "<<basic<<endl<<"HRA: "<<hra<<endl<<"Gross Salary: "<<basic + hra + 5000<<endl<<"***"<<endl;
        }
        void calculateGross(int basic, int hra, int da)
        {
            cout<<"Basic: "<<basic<<endl<<"HRA: "<<hra<<endl<<"DA: "<<da<<endl<<"Gross Salary: "<<basic + hra + da + 5000<<endl<<"***"<<endl;
        }
        void calculateGross(int basic, int hra, int da, int ta)
        {
            cout<<"Basic: "<<basic<<endl<<"HRA: "<<hra<<endl<<"DA: "<<da<<endl<<"TA: "<<ta<<endl<<"Gross Salary: "<<basic + hra + da + ta + 5000<<endl<<"***"<<endl;
        }
};

int main()
{
    Employee E;
    E.printData();
    E.calculateGross(15000);
    E.calculateGross(15000, 3600);
    E.calculateGross(15000, 3600, 7000);
    E.calculateGross(15000, 3600, 7000, 8500);
    return 0;
}
