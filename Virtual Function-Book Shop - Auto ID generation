/*Design a stock maintenance system for a Book Shop which acts as both lending library and a sales store. 
Design a C++ class to store and display the basic details of a book.
Bookshop contains two types of Books 1) LendingBook and 2)SalesBook. 
Inherit two classes to store and display specific information about Lending Book (Lending Date and Return Date) 
and Sales Book(Quantity, Price, Amount) Calculate Amount-=Quantity*price.  
Display a menu to get the choice from the bookstore person, what type of book he wants to add in the stock. 
According to the choice, create object for the specific class. Repeat the menu display if the bookstore person wants to continue adding books to stock.
Use Dynamic Polymorphism for binding the functions. Use static data member for automatic book id generation.  
Refer the Sample I/O for data members.
Sample Input:
1  (Choice of object)
Ikkigai 
Roy
Jan-7
Feb-7
y (Continue y/n)
2 (Choice of object)
C++
Yashvanth
3
500
y (Continue y/n)
2 (Choice of object)
C
Dennis
5
1200
n (Continue y/n)
Sample Output:
1:Lending Book
2.Sales Book
Book ID:1
Title:Ikkigai
Author:Roy
Lending Date:Jan-7
Return Date:Feb-7
 Do you want to continue? y/n
1:Lending Book
2.Sales Book
Book ID:2
Title:C++
Author:Yashvanth
Quantity3
Price:500
Amount:1500
 Do you want to continue? y/n
1:Lending Book
2.Sales Book
Book ID:3
Title:C
Author:Dennis
Quantity5
Price:1200
Amount:6000
 Do you want to continue? y/n*/


#include<iostream>
using namespace std;
class book{
    public:
    string bname,name;
    static int bookid;
    void bookinc(){
        bookid++;
    }
    void read(){
        cin>>bname>>name;
    }
    void out(){
        cout<<"\nBook ID:"<<bookid<<"\nTitle:"<<bname<<"\nAuthor:"<<name;
    }
};
int book::bookid=0;
class lend:public book{
    public:
    string dt1,dt2;
    lend(){
        book::bookinc();
    }
    void read1(){
        book::read();
        cin>>dt1>>dt2;
    }
    void out1(){
        book::out();
        cout<<"\nLending Date:"<<dt1<<"\nReturn Date:"<<dt2<<"\n";
    }
};
class sales:public book{
    public:
    int p,q;
    sales(){
        book::bookinc();
    }
    void read1(){
        book::read();
        cin>>q>>p;
    }
    void out1(){
        book::out();
        cout<<"\nQuantity:"<<q<<"\nPrice:"<<p<<"\nAmount:"<<p*q<<"\n";
    }
};
int main(){
    char choice;
    int c;
    do{
        cout<<"1.Lending Book\n2.Sales Book";
        cin>>c;
        if(c==1){
        lend o;
        o.read1();
        o.out1();
            
        }
        if(c==2){
        sales p;
        p.read1();
        p.out1();
            
        }
        cout<<"Do you want to continue? y/n\n";
        cin>>choice;
    }
    while(choice=='y');
    return 0;
}
