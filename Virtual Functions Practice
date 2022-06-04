/*This problem is to get you familiar with virtual functions. Create three classes Person, Professor and Student. 
The class Person should have data members name and age. The classes Professor and Student should inherit from the class Person.
The class Professor should have two integer members: publications and Empid. There will be two member functions: getdata and putdata. 
The function getdata should get the input from the user: the name, age and publications of the professor. 
The function putdata should print the name, age, publications and the Empid of the professor.
The class Student should have two data members: marks, which is an array of size 3  and studID. 
It has two member functions: getdata and putdata. The function getdata should get the input from the user: the name, age, and the marks of the student in 3 subjects. 
The function putdata should print the name, age, sum of the marks and the studID of the student.
For each object being created of the Professor or the Student class, sequential id's should be assigned to them starting from 1 .
Solve this problem using virtual functions, constructors and static variables.  Create two objects each for both Professor Class and Student Class.*/

/*Sample Input:
Walter 50 98
Jessie 25 15
White 18 89 96 96
Pinkman 19 54 52 45
Sample Output:
Name:Walter
Age:50
Publications:98
Professor ID:1
Name:Jessie
Age:25 
Publications:15
Professor ID:2
Name:White
Age:18
Mark1:89
Mark2:96
Mark3:96
Student ID:1
Name:Pinkman
Age:19
Mark1:54
Mark2:52
Mark3:45
Student ID:2*/

#include <iostream>

using namespace std;

class Person
{
    public:
        string name;
        int age;
        virtual void getData()
        {
            cin>>name>>age;
        }
        virtual void putData()
        {
            cout<<name<<age;
        }
};
class Professor: public Person
{
    private:
        int pub, eid;
        static int pobj;
    public:
        Professor()
        {
            pobj++;
            eid = pobj;
        }
        void getData()
        {
            cin>>name>>age>>pub;
        }
        void putData()
        {
            cout<<name<<" ";
            cout<<age<<" ";
            cout<<pub<<" ";
            cout<<"ID:"<<eid<<endl;
        }
};

int Professor::pobj = 0;

class Student: public Person
{
    private:
        int marks[3], sid;
        static int sobj;
    public:
        Student()
        {
            sobj++;
            sid = sobj;
        }
        void getData()
        {
            cin>>name>>age>>marks[0]>>marks[1]>>marks[2];
        }
        void putData()
        {
            cout<<name<<" ";
            cout<<age<<" ";
            cout<<marks[0]<<" ";
            cout<<marks[1]<<" ";
            cout<<marks[2]<<" ";
            cout<<"ID:"<<sid<<endl;
        }
};
int Student::sobj = 0;

int main()
{
    Person *ptr1, *ptr2, *ptr3, *ptr4;
    Professor p1, p2;
    Student s1, s2;
    ptr1 = &p1;
    ptr2 = &p2;
    ptr3 = &s1;
    ptr4 = &s2;
    ptr1->getData();
    ptr2->getData();
    ptr3->getData();
    ptr4->getData();
    ptr1->putData();
    ptr2->putData();
    ptr3->putData();
    ptr4->putData();
    return 0;
}
