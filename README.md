# demo
for practice
#include<iostream>
using namespace std;
template<class t1,class t2>
class base
{
    protected:
    t1 data1;
    t2 data2;
    public:
    void set(t1 a,t2 b)
    {
        data1=a;
        data2=b;
    }
    t1 call_data1()
    {
        return data1;
    }
    t2 call_data2()
    {
        return data2;
    }
};
int main()
{
    base <int,string> b1;
    int d;
    string d1;
    cout<<"enter the first data :"<<endl;
    cin>>d;
    cout<<"enter the second data :"<<endl;
    getline(cin,d1);
    b1.set(d,d1);
    cout<<"you had entered first value as "<<b1.call_data1();
    cout<<"you had entered second value as "<<b1.call_data1();
}
