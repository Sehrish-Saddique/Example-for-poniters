# Example-for-poniters
#include<iostream>
using namespace std;

void showvalue(int value[],int size)
{
   
   cout<<"\nEnter "<<size<<" inputs\n";
    for(int i=0; i<size; i++)
    {
       cin>>value[i];
    }
    cout<<"Now these inputs are:";
    for(int i=0; i<size; i++)
    {
       cout<<"\t"<<value[i];
    }
    
}
void refrencevariable(int &donuts)
{
    cout<<"\nEnter Donuts:";
    cin>>donuts;
    cout<<"\nDonuts are: "<<donuts<<endl;
}
int main() 
{
    int const SIZE=5;
    int array[SIZE],*arrayptr;
    arrayptr=array;
    int x=78,*ptrx;
    ptrx=&x;
    cout<<"\nThe value of x is: "<<x;
    cout<<"\nThe value of ptrx/address is: "<<ptrx;
    cout<<"\nThe  value of *ptrx is: "<<*ptrx;
    ptrx=ptrx+1;
    *ptrx=100;
    cout<<"\n*************************************";
    cout<<"\nThe updated value of ptrx/address after ptrx+1 is: "<<ptrx;
    cout<<"\nThe updated value of *ptrx is: "<<*ptrx;
    cout<<"\nThe updated value of x is: "<<x;
    cout<<"\n-------------------------------------";


    showvalue (array,SIZE);
    cout<<"\nThe derefrence array first element is is: "<<*array<<endl;
    cout<<"Size of arrayptr is: "<<sizeof(arrayptr)<<endl;
    cout<<"Size of array is: "<<sizeof(array)<<endl;

    cout<<"\nThe value of aray+1 is: "<<*(array+1);
    cout<<"\nThe value of aray+2 is: "<<*(array+2);
    cout<<"\nThe value of aray+3 is: "<<*(array+3);
    cout<<"\nThe value of aray+4 is: "<<*(array+4);
    cout<<"\nThe value of aray+0 is: "<<*(array+0);
    cout<<"\n*************************************";

    cout<<"\nThe value of arayptr+1 is: "<<*(arrayptr+1);
    cout<<"\nThe value of arayptr+2 is: "<<*(arrayptr+2); 
    cout<<"\nThe value of arayptr+3 is: "<<*(arrayptr+3);
    cout<<"\nThe value of arayptr+4 is: "<<*(arrayptr+4);
    cout<<"\nThe value of arayptr+0 is: "<<*(arrayptr+0);
    cout<<"\n*************************************";

    cout<<"\nThe value of aray[0] is: "<<array[0];
    cout<<"\nThe value of aray[1] is: "<<array[1];
    cout<<"\nThe value of aray[2] is: "<<array[2];
    cout<<"\nThe value of aray[3] is: "<<array[3];
    cout<<"\nThe value of aray[4] is: "<<array[4];
    cout<<"\n*************************************";

    cout<<"\nThe value of aray[0] is: "<<arrayptr[0];
    cout<<"\nThe value of aray[1] is: "<<arrayptr[1];
    cout<<"\nThe value of aray[2] is: "<<arrayptr[2];
    cout<<"\nThe value of aray[3] is: "<<arrayptr[3];
    cout<<"\nThe value of aray[3] is: "<<arrayptr[4];
    cout<<"\n*************************************";

    
     int jellydonuts;
     refrencevariable(jellydonuts);
     cout<<"Jelly donuts are: "<<jellydonuts<<endl;
    return 0;

}
