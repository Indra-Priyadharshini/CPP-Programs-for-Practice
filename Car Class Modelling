/*Class: Car

Private Data Members: Colour, Name, Manufacturer, Mileage, Yearmodel

Public Member Functions: default constructor, readCar(), setCar(char*,char*,char*,float,int), printCar() const

Create the following objects:

 object C1, call readCar() and printCar() functions

object C2, call setCar() with the values(Black,i10,Hyundai,20.36,2012) and printCar() functions.

Constant object C3 and call printCar() function.*/

#include <iostream>
#include <string>

using namespace std;

class Car
{
    private:
        int year;
        float mil;
        string col, name, man;
    public:
        Car()
        {
            col = "*  ";
            name = '*';
            man = '*';
            mil = 0;
            year = 0;
        }
        void readCar()
        {
            cin>>col>>name>>man>>mil>>year;
        }
        //(Black,i10,Hyundai,20.36,2012)
        void setCar(char* co, char* na, char* ma, float mi = 20.36, int ye = 2012)
        {
            string tempcol, tempname, tempman;
            for (int i=0; *(co + i)!='\0'; i++) tempcol += *(co + i);
            col = tempcol;
            for (int i=0; *(na + i)!='\0'; i++) tempname += *(na + i);
            name = tempname;
            for (int i=0; *(ma + i)!='\0'; i++) tempman += *(ma + i);
            man = tempman;
            mil = mi;
            year = ye;
        }
        void printCar() const
        {
            cout<<"Colour: "<<col<<endl;
            cout<<"Name: "<<name<<endl;
            cout<<"Manufacturer: "<<man<<endl;
            cout<<"Mileage: "<<mil<<endl;
            cout<<"Yearmodel: "<<year<<endl;
        }
};

int main()
{
    Car c1;
    c1.readCar();
    c1.printCar();
    
    Car c2;
    c2.setCar("Black","i10","Hyundai",20.36,2012);
    c2.printCar();
    
    const Car c3;
    c3.printCar();
    return 0;
}
