//Task-1(Number guessing game)

#include <cstdlib>
#include <iostream>
using namespace std;
int main()
{
    int m=rand();
    int n;
    cout<<"guess the number"<<endl;
    cout<<"hint: it's a two digit number"<<endl;
    if(n==m)
    cout<<"you have guessed the number right!";
    while(n!=m)
    {
    cout<<endl<<"guess the number"<<endl;
    cin>>n;
    if(n<m-31 || n>m+58)
    cout<<"wrong choice!";
    if(n<=m-16)
    cout<<"too low for the correct number";
    else if(n>m-16 && n<=m-3)
    cout<<"still low";
    else if(n>m-3 && n<=m-1)
    cout<<"too close but still low";
    else if(n>m+25 && n<=m+58)
    cout<<"too high for the correct number";
    else if(n>m+5 && n<=m+25)
    cout<<"still high";
    else if(n>m && n<=m+5)
    cout<<"too close but still high";
    }
    cout<<"congrats,you have guessed the number right!";
    return 0;
}
