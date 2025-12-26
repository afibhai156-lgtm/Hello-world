//Temperature converter

#include<iostream>
using namespace std;
int main()
{
    double c,f,k;
    int choice;
    do {
        cout << "Temperature converter" << endl;
        cout << "convrt" << endl;
        cout << "1.calsius to fehranhiet" << endl;
        cout << "2.fehranhiet to calsius" << endl;
        cout << "3.calsius to kelvin" << endl;
        cout << "4.kelvin to calcius" << endl;
        cout << "5.fehrrennhiet to kelvin" << endl;
        cout << "6.kelvin to fehranhiet" << endl;
        cout << "7.exit" << endl;
        cout << "enter you choice(1_7)" << endl;
        cin >> choice;
        switch (choice) {
        case 1:
            cout << "enter temp in calsius" << endl;
            cin >> c;
            f=c*(9.0/5.0)+32;
            cout <<f <<"fehranhiet temp" << endl;
            break ;
        case 2:
            cout << "fehrrennhiet to calsius" << endl;
            cin >> f;
            c=f-32*(5.0/9.0);
            cout <<c<< "calsius" << endl;
            break;
        case 3:
            cout << "calsius to kelvin" << endl;
            cin >> c;
            k=273.15+c;
            cout <<k<<" kelvin" << endl;
            break;
        case 4:
            cout << "kelvin to calsius" << endl;
            cin >> k;
            c=k-273.15;
            cout <<k<< "casius" << endl;
            break ;
        case 5:
            cout << " fehrrennhiet to kelvin" << endl;
            cin >> f;
            k=f-32*(5.0/9.0)+273.15;
            cout<<k << "kelvin" << endl;
            break;
        case 6:
            cout << "kelvin to fehrrennhiet" << endl;
            cin >> k;
            f=k-273.15*(9.0/5.0)+32;
            cout <<f<< "fehrrennhiet" << endl;
            break;
        case 7:
            cout << " Good bye" << endl;
            break;
        default :
            cout << "invalid choice !please enter (1_7)" << endl;
        }
    } while( choice!=7);
    return 0;
}

