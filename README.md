# Repository_for_binary_decrement-
operator -- for time C++ Oop
#include <iostream>
using namespace std;
class Time
{
private:
int h, m, s;
public:
Time()
{
h = m = s = 0;
}

Time(int hh, int mm, int ss)
{
h = hh;
m = mm;
s = ss;
}
void operator --(int mm)
{
if(mm==0)
{
m=59;
h--;
}
else

m--;
}
void show()
{
cout<<h<<"Hours-"<<m<<"Minutes-"<<s<<"Seconds"<<endl;

}
};
int main()
{
Time obj (00,10,50);
cout<<"Intial Values of Time"<<endl;
obj.show();
obj--;
cout<<"After -- Operator"<<endl;
obj.show();
return 0;
}
