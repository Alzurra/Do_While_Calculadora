# Do_While_Calculadora
C++

#include <iostream>
#include <iomanip>

using namespace std;

int main(){
	

	float n1;
	float n2;
	float r;
	float div;
	char op;
	float resposta;
	
do{
	cout<<"Digite o primeiro numero:";
	cin>>n1;
	cout<<"Digite o segundo numero:";
	cin>>n2;
	cout<<endl;
	cout<<"****CALCULDADORA****"<<endl;
	cout<<endl;
	cout<<" [1] SOMA"<<endl;
 	cout<<" [2] SUBTRACAO"<<endl;
 	cout<<" [3] MULTIPLICACAO"<<endl;
 	cout<<" [4] DIVISAO"<<endl;
	cout<<endl;
	cout<<"Digite a opcao a ser realizada:";
	cin>>op;
	
	switch(op)
	{
	case '1':
		r = n1 + n2;
		cout<<setprecision(2)<<endl;
		cout<<"RESULTADO:"<<r<<endl;
		break;
	case '2':
		r = n1 - n2;
		cout<<setprecision(2)<<endl;
		cout<<"RESULTADO:"<<r<<endl;
		break;
	case '3':
		r = n1 * n2;
		cout<<"RESULTADO:"<<r<<endl;
		break;
	case '4':
		if(n2!=0)
		{
			div = n1 / n2;
			cout<<setprecision(2)<<endl;
			cout<<"RESULTADO:"<<div<<endl;
		}
		else
		{
			cout<<"DIVISAO POR ZERO!!!"<<endl;
		}
		break;
	default:
	break;
	}
	cout<<"Deseja realizar outra operacao? [1] SIM [2] NAO"<<endl;
	cin>>resposta;
	cout<<endl;
	if(resposta ==1)
	{
		cout<<"OUTRA OPERACAO!!"<<endl;	
	}
	else
	{
	 cout<<"PROGRAMA FINALIZADO!!"<<endl;	
	}
  }
	while (resposta == 1);
	
	return 0; 
}      
