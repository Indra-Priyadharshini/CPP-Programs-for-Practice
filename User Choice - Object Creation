/*This problem is to get you familiar with virtual functions. Create three classes Person, Professor and Student.
The class Person should have data members name and age. The classes Professor and Student should inherit from the class Person.
The class Professor should have two integer members: publications and Empid. 
There will be two member functions: getdata and putdata. The function getdata should get the input from the user: the name, age and publications of the professor. 
The function putdata should print the name, age, publications and the Empid of the professor.
The class Student should have two data members: marks, which is an array of size 3  and studID. 
It has two member functions: getdata and putdata. The function getdata should get the input from the user: the name, age, and the marks of the student in 3 subjects. 
The function putdata should print the name, age, sum of the marks and the studID of the student.
For each object being created of the Professor or the Student class, sequential id's should be assigned to them starting from 1 .
Solve this problem using virtual functions, constructors and static variables.  Create objects according to the user choice - 1 for Professor and 2 for Student'

Sample Input:
The first line reads the user choice for creating the object. The next line is the input for the respective object.
1
Walter 50 98
1
Jessie 25 15
2
White 18 89 96 96
2
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
Student ID:2 */

#include <iostream>

using namespace std;

class Person
{
    private:
        int age;
        string name;
    public:
        Person()
        {
            age = 0; name = "";
        }
        virtual void getData()
        {
            cin>>name>>age;
        }
        virtual void putData()
        {
            cout<<"Name:"<<name<<endl;
            cout<<"Age:"<<age<<endl;
        }
};

class Professor: public Person
{
    private:
        static int empid;
        int pub;
    public:
        Professor()
        {
            empid++;
        }
        void getData()
        {
            cin>>pub;
        }
        void putData()
        {
            cout<<"Publications:"<<pub<<endl;
            cout<<"Professor ID:"<<empid<<endl;
        }
};

class Student: public Person
{
    private:
        int marks[3];
        static int studid;
    public:
        Student()
        {
            studid++;
        }
        void getData()
        {
            cin>>marks[0]>>marks[1]>>marks[2];
        }
        void putData()
        {
            cout<<"Mark1:"<<marks[0]<<endl;
            cout<<"Mark2:"<<marks[1]<<endl;
            cout<<"Mark3:"<<marks[2]<<endl;
            cout<<"Student ID:"<<studid<<endl;
        }
};

int Professor::empid = 0;
int Student::studid = 0;

int main()
{
    for (int i=0; i<4; i++)
    {
        int ch;
        cin>>ch;
        Person* ptr;
        Person per;
        ptr = &per;
        ptr->getData();
        if (ch==1)
        {
            Professor pro;
            ptr = &pro;
            ptr->getData();
            ptr = &per;
            ptr->putData();
            ptr = &pro;
            ptr->putData();
        }
        else
        {
            Student stu;
            ptr = &stu;
            ptr->getData();
            ptr = &per;
            ptr->putData();
            ptr = &stu;
            ptr->putData();
        }
    }
    return 0;
}
