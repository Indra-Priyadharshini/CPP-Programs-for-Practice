/*Class: Complex

Private Data Members: Real, Imaginary

Public Member Functions:

Complex() - Default constructor

Complex (Complex&) - Copy Constructor

readData() - to read data

printData() - to print it in the given format - a+bi (a-real part, b - imaginary part)

Overload + opertor to add two complex objects and store the result in the first Complex object.

Overload - operator to sutract two complex objects and return the result. Reterive the result and store it in the new object in main function.

Define main() to create 3 objects, C1, C2 and C3. Call relevant member functions to read data for C1 and C2. Add C1 and C2, print the sum. 
Subtract C1 from C2, store it in C3, print the difference. 
Sample Input:
5 6
4 3
Sample Output:
5+6i
4+3i
Sum: 9+9i
Difference: 5+6i*/

#include <iostream>

using namespace std;

class Complex
{
    private:
        int Real, Imag;
    public:
        Complex();
        Complex(const Complex&);
        void readData();
        void printData();
        void operator +(Complex);
        Complex operator -(Complex);
};

Complex::Complex()
{
    Real = 0;
    Imag = 0;
}
Complex::Complex(const Complex& C1)
{
    Real = C1.Real;
    Imag = C1.Imag;
}
void Complex::readData() { cin>>Real>>Imag; }
void Complex::printData() { cout<<Real<<(Imag<0? "" : "+")<<Imag<<"i"<<endl; }
void Complex::operator +(Complex C1)
{
    Real += C1.Real;
    Imag += C1.Imag;
}
Complex Complex::operator -(Complex C1) 
{
    Complex C2;
    C2.Real = Real - C1.Real;
    C2.Imag = Imag - C1.Imag;
    return C2;
}

int main()
{
    Complex c1, c2;
    c1.readData();
    c2.readData();
    c1.printData();
    c2.printData();
    c1 + c2;
    cout<<"Sum: ";
    c1.printData();
    Complex c3 = c1 - c2;
    cout<<"Difference: ";
    c3.printData();
    return 0;
}
