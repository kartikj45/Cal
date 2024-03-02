#include<stdio.h>
#include<iostream>
#include<math.h>
using namespace std;
int main()
{
	float a,b,i=2;
	char x;
	while(i!=0){
	scanf("%f %c %f",&a,&x,&b);
	int j=a;
	int k=b;
	float yy=a-j;
	float zz=a-k;
	switch(x){
		case '+':{
			if((yy>0 || yy<0)|| (zz>0 || zz<0)){
			cout<<a+b<<endl<<endl;}
			else{
				cout<<j+k<<endl<<endl;
			}
			break;
		}
	    case '-':
			if((yy>0 || yy<0)|| (zz>0 || zz<0)){
			cout<<a-b<<endl<<endl;}
			else{
				cout<<j-k<<endl<<endl;
			}
			break;	
		case '*':
			if((yy>0 || yy<0)|| (zz>0 || zz<0)){
			cout<<a*b<<endl<<endl;}
			else{
				cout<<j*k<<endl<<endl;
			}
			break;
		case '/':{
			int r=a/b;
			float t=(a/b)-r;
			if(t>0 || t<0){
			cout<<a/b<<endl<<endl;}
			else{
				cout<<r<<endl<<endl;
			}
			
			
			break;}	
		case '%':
			cout<<j%k<<endl<<endl;
			break;
		case '^':
		    cout<<pow(a,b)<<endl<<endl;
			break;	
		case '@':
		    cout<<sqrt(a)<<endl<<endl;
			break;
		case 'm':
		    cout<<"For addition -> (num1 + num2).\nFor Subtraction -> (num1 - num2).For multiplication -> (num1 * num2).\nFor division -> (num1 / num2).\nFor Modulus/Reaminder -> (num1 % num2).\nFor power -> (num ^ power).\nFor square root -> (num @ 0)."<<endl<<endl;
			break;	
		default:
		    cout<<"Not valid operation.\nOpen menu by pressing 3m3"<<endl<<endl;
			break;		
	}
	i++;
	}
	return 0;
	
}
