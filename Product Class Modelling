/*Create a class product with following specifications:

Private Data Members: Pno, Pname, Pdesc, Pprice, Pcategory (Pcategory can take any of the follwing values:  Premium, Basic, Standard)

Private static data member : Product_count

private member function: display_Bonus() - Calculate the Bonus based on the following conditions.

If category is Premium, Bonuspts=100, If category is Standard, Bonuspts=50, If category is Basic, Bonuspts=10.

Public Member Functions: Default constructor, Argumented Constructor, Copy constructor.

readProduct(), printProduct() const, calcBill(int units) - function to calculate and print bill amount using units and price. (Units is the argument, price is the data member), if the units argument is skipped in the function call, make the default value as 1. 

Public static member function: display_count_objects() - count the number of objects using Product_count variable and print it.

Declare 4 objects (P1, P2, P3, P4) and call the required functions to display the result as shown in testcases. 
create 5th object using existing object P1. Print the total number of objects as the last line in the output. 

Hints: 1) Call the private member function display_Bonus in calcBill() function. 2)Use classname to call the static member function.
3)Dont forget to define the static data member outside the class 4)Increment the static variable in each constructor. 5)Define the printProduct() as constant function. 6) Skip the units argument while calling calcBill() for P3. 

Sample Output:
Pno:100
Name:Soap
Description:Bathing Soap
Price:20
Category:Premium
Units:6
Amount:120
Bonus Points:100
Total Number of Objects:5*/

#include <iostream>

using namespace std;

class Product
{
    private:
        int Pno, Pprice, Bonuspts;
        string Pname, Pdesc, Pcategory;
        static int Product_count;
        
        void display_Bonus()
        {
            if (Pcategory=="Premium") Bonuspts = 100;
            else if (Pcategory=="Standard") Bonuspts = 50;
            else Bonuspts = 10;
            cout<<"Bonus Points:"<<Bonuspts<<endl;
        }
    public:
        Product()
        {
            Product_count++;
        }
        Product(Product& pro)
        {
            Pno = pro.Pno;
            Pname = pro.Pname;
            Pprice = pro.Pprice;
            Pdesc = pro.Pdesc;
            Pcategory = pro.Pcategory;
            Product_count++;
        }
        void readProduct()
        {
            cin>>Pno>>Pname>>Pdesc>>Pprice>>Pcategory;
        }
        void printProduct() const
        {
            cout<<"Pno:"<<Pno<<endl;
            cout<<"Name:"<<Pname<<endl;
            cout<<"Description:"<<Pdesc<<endl;
            cout<<"Price:"<<Pprice<<endl;
            cout<<"Category:"<<Pcategory<<endl;
        }
        void calcBill(int units = 1)
        {
            cout<<"Units:"<<units<<endl;
            int amount = Pprice * units;
            cout<<"Amount:"<<amount<<endl;
            display_Bonus();
        }
        static void display_count_objects()
        {
            cout<<"Total Number of Objects:"<<Product_count<<endl;
        }
};

int Product::Product_count = 0;

int main()
{
    Product p1, p2, p3, p4;
    p1.readProduct();
    p1.printProduct();
    p1.calcBill(6);
    p2.readProduct();
    p2.printProduct();
    p2.calcBill(100);
    p3.readProduct();
    p3.printProduct();
    p3.calcBill();
    p4.readProduct();
    p4.printProduct();
    p4.calcBill(5);
    Product p5(p1);
    p5.printProduct();
    p5.calcBill(6);
    
    Product::display_count_objects();
    
    return 0;
}
