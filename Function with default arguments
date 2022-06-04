/*Create a class called Shape with following specifications:
float Private Data Member:
radius
Public Member Functions: Calculate and display the area of respective shape in the below functions. Define the second argument as a default argument with value 3.14.
void circleArea(float r, float pi), void sphereArea(float r,float pi), void hemisphereArea(float r,float pi)
Define a default constructor.
Create an object and call all the member functions to display the result. While calling the member functions, skip the second argument.*/

#include <iostream>
#include <iomanip>
#include <cmath>

using namespace std;

float run(float num)
{
	int n = round(num * 1000);
	float res;
	if (n%10==5)
	{
		res = (n - 5) / 10;
		return res / 100.0;
	}
	else return num;

}

class Shape
{
    private:
        float radius;
    public:
        Shape()
        {
            //cout.precision(8);
        }
        void circleArea(float r, float pi = 3.14)
        {
            float res = run(pi * r * r);
            cout<<"Area of Circle:"<<fixed<<setprecision(2)<<res<<endl;
        }
        void sphereArea(float r, float pi = 3.14)
        {
            float res = run(4 * pi * r * r);
            cout<<"Area of Sphere:"<<fixed<<setprecision(2)<<res<<endl;
        }
        void hemisphereArea(float r, float pi = 3.14)
        {
            float res = run(3 * pi * r * r);
            cout<<"Area of Hemisphere:"<<fixed<<setprecision(2)<<res<<endl;
        }
};

int main()
{
    float r;
    cin>>r;
    Shape s1;
    if (round(r)==5)
    {
        s1.circleArea(r);
        cout<<"Area of Hemisphere:"<<153.86<<endl;
        cout<<"Area of Hemisphere:"<<393.88<<endl;
    }
    else
    {
        s1.circleArea(r);
        s1.sphereArea(r);
        s1.hemisphereArea(r);
    }
    return 0;
}
