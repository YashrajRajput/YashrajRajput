/*

Name :- Yashraj Rajput

Username :- YashrajRajput

Project Name :- Simple Calculator (C++ Program Code)

*/





#include<iostream>
#include<cmath>
using namespace std;

class simple
{
    float a, b;

public:
    float ans;
    int ch;

    void setdata(float c, float d)
    {
        a = c;
        b = d;
    }
    void displaydata()
    {
        cout << "1st number is = " << a << endl;
        cout << "2nd number is = " << b << endl;
    }

    void simplecalcy()
    {
        cout << "menu :"
             << "\n"
             << "1.addition"
             << "\n"
             << "2.substraction"
             << "\n"
             << "3.multiplication"
             << "\n"
             << "4.division"
             << "\n";

        cout << "enter your choice = " ;
        cin >> ch;

        switch (ch)
        {
        case 1:
            ans = a + b;
            break;

        case 2:
            ans = a - b;
            break;

        case 3:
        ans = a*b;
        break;

        case 4:
        ans = a/b;
        break;
        }
    cout << " the answer of given question is = " << ans << endl ;
    }

};


class scical
{
    float j ;
    public:
    int ch ;
    float key ;
    
    void setnum(float d)
    {
        j = d ;
    }    
    void shownum()
    {
        cout << "your number is = " << j << endl ;
    }

    void scicalcy()
    {
        cout << "menu :" << endl << "1.sin(in radian)" << endl << "2.cos(in radian)" << endl << "3.tan(in radian)" << endl << "4.log(to base e)" << endl ;
        cout << "enter your choice = " ;
        cin >> ch ;

        switch(ch)
        {
            case 1:
            key = sin(j);
            break ;

            case 2:
            key = cos(j);
            break ;

            case 3:
            key = tan(j);
            break ;

            case 4:
            key = log(j);
            break ;
        }
        cout << "The answer is = " << key << endl ;
    }

};

int main()
{
    float k,l;
    cout << "enter value for k = " ;
    cin >> k ;
    cout << "enter value for l = " ;
    cin >> l ;
    simple y;
     y.setdata(k, l);
     y.displaydata();
     y.simplecalcy();

    scical z;
    z.setnum(k);
    z.shownum();
    z.scicalcy();
    return 0;
}
