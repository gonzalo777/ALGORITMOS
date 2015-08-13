#include <iostream>
#include "conio.h"
#include "math.h"
#include "stdlib.h"

using namespace std;

void main(){
int op=0,l,prom,x,y,z,a,b,res,area;
do{
cout<<"-------MENU------\n";
cout<<"1.-Area del cuadrado \n";
cout<<"2.-Promedio de 3 numeros \n";
cout<<"3.-Mayor de dos numeros \n";
cout<<"4.-Salir\n";
cin>>op;
switch(op){
case 1: cout<<"Ingrese el lado del cuadrado\n";
	cin>>l;
	area=l*l;
	cout<<"el area es:\n"<<area<<endl;
	break;
case 2: cout<<"Ingrese el primer numero :\n";
		cin>>x;
		cout<<"Ingrese el segundo numero :\n";
		cin>>y;
		cout<<"Ingrese el tercer numero :\n";
		cin>>z;
		prom=(x+y+z)/3;
		cout<<"El promedio es: \n"<<prom<<endl;
		break;
case 3: cout<<"Ingrese un numero \n";
		cin>>a;
		cout<<"Ingrese el otro numero \n";
		cin>>b;
		if(a>b)
			res=b;
		else(b>a);
			res=a;
		cout<<"el numero mayor es : \n"<<res<<endl;
		break;
default: break;
}
}while(op!=4);
getch();
system("cls");


}
