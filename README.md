#include<iostream>
using namespace std;

namespace foo{
	int doSomething(int x, int y){
		return x+y;
	}
}
namespace goo{
	int doSomething(int x, int y)//forward declaration
{
	return x-y;
		
}
}
int main(){
	cout<<foo::doSomething(4,3)<<'\n';//cual dosomething llamara?
	return 0;
}

