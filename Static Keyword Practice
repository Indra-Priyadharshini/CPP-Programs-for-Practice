/*Class: Box

Private Data Members: Length, Breadth, Height

Static Data Member: Box_Count

Constructors: Box() - Assign default values to data members and increment the Box_Count. 

Public Member Functions: readData() - to read values for object, calcVolume() - to calculate and display the volume of cuboid box

Static Member Function: display() - to display the Box_Count value.

Objects:

B1, B2, B3 - Call the readData() and calcVolume() for each object and finally call display().*/

#include <iostream>

using namespace std;

class Box
{
    private:
        int length, breadth, height;
    public:
        static int Box_Count;
        Box()
        {
            length = 5; 
            breadth = 5; 
            height = 5; 
            Box_Count++;
        }
        void readData()
        {
            cin>>length>>breadth>>height;
        }
        void calcVolume()
        {
            int res = length * breadth * height;
            cout<<"Volume = "<<res<<endl;
        }
        static void display()
        {
            cout<<"Number of Boxes: "<<Box_Count<<endl;
        }
    
};

int Box::Box_Count = 0;

int main()
{
    Box b1, b2, b3;
    b1.readData();
    b1.calcVolume();
    b2.readData();
    b2.calcVolume();
    b3.readData();
    b3.calcVolume();
    b3.display();
    
    return 0;
}
